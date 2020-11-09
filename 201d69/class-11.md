# Code 201
## Reading 10

### HTML & CSS
#### Images (pp. 406-427)
* CSS can change the dimensions of an image
* Images can be aligned both horizontally and vertically
* You can use a background image for any box element on the page
* You can choose to have the background image show only once or repeat
* you can create image rollover effects by moving the position of the image
* you can create image sprites to reduce the number of images a browser needs to load

#### Practical Information (pp. 476-492)
* Search Engine optimization helps users find your sites through searches on the internet
* Analytics Tools (i.e. Google Analytics) let you see the metrics for visitor experience
  1. How many visitors
  1. Visitor satisfaction
  1. How visitor uses your site
* A Web Hosting Service and Domain Name is required to put your web site on the internet
* FTP (File Transfer Protocol) allows you to move files from your local machine to Web Server
* Many Web Hosting Services provide tools to help you design your site.
  1. blogging
  1. email
  1. newsletters
  1. e-commerce

  #### Flash (pp. 201-206)
  * Flash was used since the late 1990s to create animations, play audio, and play video in websites.
  * Since 2005 use of Flash has been in decline.

  [Video and Audio APIs](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Client-side_web_APIs/Video_and_audio_APIs)
  * HTML5 comes with elements to allow the embedding of media (audio/video) in documents
  * Requires the knowledge of basic JavaScript to use
  * HTMLMediaElement provides features to allow you to control video and audio playback
    1. HTMLMediaElement.play()
    1. HTMLMediaElement.pause()
    1. \<audio\>
    1. \<video\>
    ```
    ======================================================================================================================
    Sample HTML Code | https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Client-side_web_APIs/Video_and_audio_APIs   
    ======================================================================================================================

    <div class="player">
      <video controls>
        <source src="video/sintel-short.mp4" type="video/mp4">
        <source src="video/sintel-short.webm" type="video/webm">
        <!-- fallback content here -->
      </video>
      <div class="controls">
        <button class="play" data-icon="P" aria-label="play pause toggle"></button>
        <button class="stop" data-icon="S" aria-label="stop"></button>
        <div class="timer">
          <div></div>
          <span aria-label="timer">00:00</span>
        </div>
        <button class="rwd" data-icon="B" aria-label="rewind"></button>
        <button class="fwd" data-icon="F" aria-label="fast forward"></button>
      </div>
    </div>
    
    =====================================================================================================================
    Sample CSS Code | https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Client-side_web_APIs/Video_and_audio_APIs   
    =====================================================================================================================

    .controls {
      visibility: hidden;
      opacity: 0.5;
      width: 400px;
      border-radius: 10px;
      position: absolute;
      bottom: 20px;
      left: 50%;
      margin-left: -200px;
      background-color: black;
      box-shadow: 3px 3px 5px black;
      transition: 1s all;
      display: flex;
    }

    .player:hover .controls, player:focus .controls {
      opacity: 1;
    }

    ============================================================================================================================
    Sample JavaScript Code | https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Client-side_web_APIs/Video_and_audio_APIs   
    ============================================================================================================================

    let intervalFwd;
    let intervalRwd;

    function mediaBackward() {
      clearInterval(intervalFwd);
      fwd.classList.remove('active');

      if(rwd.classList.contains('active')) {
        rwd.classList.remove('active');
        clearInterval(intervalRwd);
        media.play();
      } else {
        rwd.classList.add('active');
        media.pause();
        intervalRwd = setInterval(windBackward, 200);
      }
    }

    function mediaForward() {
      clearInterval(intervalRwd);
      rwd.classList.remove('active');

      if(fwd.classList.contains('active')) {
        fwd.classList.remove('active');
        clearInterval(intervalFwd);
        media.play();
      } else {
        fwd.classList.add('active');
        media.pause();
        intervalFwd = setInterval(windForward, 200);
      }
    }
  ```


[<-- Back](../README.md)
