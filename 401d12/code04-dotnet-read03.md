# Code 401
## Reading 03
##### (All My Notes are attributed/sourced from the Resources directly preceding them.)

<br>
<br>
<br>

### __File and Stream I/O__
#### Author:  Microsoft Docs
[Article Source](https://docs.microsoft.com/en-us/dotnet/standard/io/)
> File and stream I/O (input/output) refers to the transfer of data either to or from a storage medium.

* System.IO namespace in C# enables reading and writing to datastreams and files.
* Commonly used file and directory classes:
  * File
  * FileInfo
  * Directory
  * DirectoryInfo
  * Path
* The Stream abstract class supports reading and writing bytes.
* Streams involve 3 fundamental operations:
  * Reading
  * Writing
  * Seeking
* Commonly used Stream classes:
  * FileStream
  * IsolatedStorageFileStream
  * MemoryStream
  * BufferedStream
  * NetworkStream
  * PipeStream
  * CryptoStream
* System.IO provides several reader and writer classes.  Examples of commonly used classes below:
  * BinaryReader / BinaryWriter
  * StreamReader / StreamWriter
  * StringReader / StringWriter
  * TextReader / TextWriter
* System.IO provides Compression and Decompression classes to help with the transfer of data
* Commonly used Compression classes:
  * ZipArchive
  * ZipArchiveEntry
  * ZipFile
  * ZipFileExtensions
  * DeflateStream
  * GZipStream
* Isolated Storage is a way to keep your application within the control of a computer's security policy.
* Commonly used Isolated Storage classes:
  * IsolatedStorage
  * IsolatedStorageFile
  * IsolatedStorageFileStream

<br>
<br>

### __How to: Write text to a file__
#### Author:  Microsft Docs
[Article Source](https://docs.microsoft.com/en-us/dotnet/standard/io/how-to-write-text-to-a-file)
* Below are common methods used to write to a text file
  * StreamWriter
  * File
  * Path

> Example: Synchronously write text with StreamWriter

```
using System;
using System.IO;

class Program
{
    static void Main(string[] args)
    {

        // Create a string array with the lines of text
        string[] lines = { "First line", "Second line", "Third line" };

        // Set a variable to the Documents path.
        string docPath =
          Environment.GetFolderPath(Environment.SpecialFolder.MyDocuments);

        // Write the string array to a new file named "WriteLines.txt".
        using (StreamWriter outputFile = new StreamWriter(Path.Combine(docPath, "WriteLines.txt")))
        {
            foreach (string line in lines)
                outputFile.WriteLine(line);
        }
    }
}
// The example creates a file named "WriteLines.txt" with the following contents:
// First line
// Second line
// Third line
```

> Example: Synchronously append text with StreamWriter

```
using System;
using System.IO;

class Program
{
    static void Main(string[] args)
    {

        // Set a variable to the Documents path.
        string docPath = Environment.GetFolderPath(Environment.SpecialFolder.MyDocuments);

        // Append text to an existing file named "WriteLines.txt".
        using (StreamWriter outputFile = new StreamWriter(Path.Combine(docPath, "WriteLines.txt"), true))
        {
            outputFile.WriteLine("Fourth Line");
        }
    }
}
// The example adds the following line to the contents of "WriteLines.txt":
// Fourth Line
```

> Example: Asynchronously write text with StreamWriter

```
using System;
using System.IO;
using System.Threading.Tasks;

class Program
{
    static async Task Main()
    {
        // Set a variable to the Documents path.
        string docPath = Environment.GetFolderPath(Environment.SpecialFolder.MyDocuments);

        // Write the specified text asynchronously to a new file named "WriteTextAsync.txt".
        using (StreamWriter outputFile = new StreamWriter(Path.Combine(docPath, "WriteTextAsync.txt")))
        {
            await outputFile.WriteAsync("This is a sentence.");
        }
    }
}
// The example creates a file named "WriteTextAsync.txt" with the following contents:
// This is a sentence.
```

> Example: Write and append text with the File class

```
using System;
using System.IO;

class Program
{
    static void Main(string[] args)
    {
        // Create a string with a line of text.
        string text = "First line" + Environment.NewLine;

        // Set a variable to the Documents path.
        string docPath = Environment.GetFolderPath(Environment.SpecialFolder.MyDocuments);

        // Write the text to a new file named "WriteFile.txt".
        File.WriteAllText(Path.Combine(docPath, "WriteFile.txt"), text);

        // Create a string array with the additional lines of text
        string[] lines = { "New line 1", "New line 2" };

        // Append new lines of text to the file
        File.AppendAllLines(Path.Combine(docPath, "WriteFile.txt"), lines);
    }
}
// The example creates a file named "WriteFile.txt" with the contents:
// First line
// And then appends the following contents:
// New line 1
// New line 2
```

<br>
<br>

### __How to: Read and write to a newly created data file__
#### Author:  Microsoft Docs
[Article Source](https://docs.microsoft.com/en-us/dotnet/standard/io/how-to-read-and-write-to-a-newly-created-data-file)
* BinaryWriter and BinaryReader are used for writing data that is not character strings.

> The following example shows how to create an empty file stream, write data to it, and read data from it.

```
using System;
using System.IO;

class MyStream
{
    private const string FILE_NAME = "Test.data";

    public static void Main()
    {
        if (File.Exists(FILE_NAME))
        {
            Console.WriteLine($"{FILE_NAME} already exists!");
            return;
        }

        using (FileStream fs = new FileStream(FILE_NAME, FileMode.CreateNew))
        {
            using (BinaryWriter w = new BinaryWriter(fs))
            {
                for (int i = 0; i < 11; i++)
                {
                    w.Write(i);
                }
            }
        }

        using (FileStream fs = new FileStream(FILE_NAME, FileMode.Open, FileAccess.Read))
        {
            using (BinaryReader r = new BinaryReader(fs))
            {
                for (int i = 0; i < 11; i++)
                {
                    Console.WriteLine(r.ReadInt32());
                }
            }
        }
    }
}


// The example creates a file named "Test.data" and writes the integers 0 through 10 to it in binary format.
// It then writes the contents of Test.data to the console with each integer on a separate line.
```

<br>
<br>
<br>

[<-- Back](../README.md)
