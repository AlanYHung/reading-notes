# Code 201
## Reading 13
##### (All My Notes are attributed/sourced from the Resources directly preceding them.)

[Local Storage](http://diveinto.html5doctor.com/storage.html)
* In the past, Local Storage did not exist for Browsers
* The beginning of Local Storage was started by MS as part of [DHTML Behaviors](http://msdn.microsoft.com/en-us/library/ms531078(v=VS.85).aspx) called userData
  * userData allowed for 64 KB of memory but did not allow give permissions to the developer to increase the size if needed
* In 2002 Adobe introduced Flash which allowed for 100 KB using [Local Shared Objects ("Flash Cookies")](http://kb2.adobe.com/cps/161/tn_16194.html).
  * Brad Neuberg developed a Flash to JavaScript Bridge called [AMASS (AJAX Massive Storage System)](http://codinginparadise.org/weblog/2005/10/amass-ajax-massive-storage-system.html)
* In 2007 Google introduced [Gears](http://gears.google.com/) a tool that can store unlimited amounts of data in SQL database tables.
* Eventually it has all evolved into what is now called "Local Storage" which is native to all modern browsers.
* Storage memory max is set to 5 MB
* Local Storage can be managed by Event Handlers using the following Methods
  1. setItem()
  1. removeItem()
  1. clear()
* Local Storage is still evolving and there are competing ideologies such as Google Gears.


[<-- Back](../README.md)
