# Code 301
## Reading 13
##### (All My Notes are attributed/sourced from the Resources directly preceding them.)


### Sending Form Data
#### Author:  Mozilla and Individual Contributors
[Article Source](https://developer.mozilla.org/en-US/docs/Learn/Forms/Sending_and_retrieving_form_data)
* The web at most basic is a server/client relationship
  * Clients sends requests to servers using HTTP protocol
  * Servers answers using the same protocol
* Forms are just user friendly ways to send requests to servers on the web
* Form tags have several attributes that help direct and receive data
  * action attribute that defines where the data is sent
  * method attributes defines the way the data 
    * get method is used by the browser to request resources from the server and is appended to the url
    * post method is used by the browser to requst resources from the server and is appended to the http body
* You have to use browser develper tools to see HTTP requests/responses sent by clients/servers
* HTTP keeps it's data in key value pairs
* Sending files are special cases as HTTP is a text protocol and files are binary
  * Set the method attribute to POST
  * Set enctype attribute to mulitpart/form-data
  * \<input type="file"\> to allow users to upload files
* Always be aware of how you handle the data as Security is very important
  * Escape potentialy dangerous characters - Need to be on the lookout for any characters that look like executable code
  * Limit the incoming amount of data to only what is necessary
  * Sandbox uploaded files - isolate the files on a completely different server than your host server



### Styling a HTML 5 Form
#### YouTube Channel:  The Net Ninja
[Article Source](https://www.youtube.com/playlist?list=PL4cUxeGkcC9g5_p_BVUGWykHfqx6bb7qK)
* letter-spacing in forms to space out the text for each word
* input[type = "radio"] - allows you to style the radio buttons
  * to replace the radio buttons set opacity to 0
  * give the labels 26px space to give room for your own radio buttons
  * cursor allows you to control pointer animation
  * put custom checked radios as background and adjust the background-position based on what is selected
* Checkboxes can be styled the same way
* You can resize and add backgrounds to input boxes that users type in.
* You can use placeholder attribut to put in default text that will be replaced as soon as user starts typing
* Use appearance: none to remove all styling to select boxes.
  * appearance is not supported the same way by all browsers so you need to do it for every browser
    1. -webkit-appearance
    1. -moz-appearance
    1. -o-appearance
    1. -ms-appearnce
    1. appearance
* With HTML 5 the required attribute allows the browser to know if you have entered something in valid format
* with CSS attach :valid to input to adjust the CSS Styling when a valid input has been entered


### Additional SQL Resources
* [HTML5 Forms Reference](https://htmlreference.io/forms/)




[<-- Back](../README.md)
