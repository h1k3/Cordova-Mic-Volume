micVolume
=========

WARNING : this plugin works in that it compiles and reads mic data, but the data read is difficult to interpret. This plugin should therefore not be treated as done, but rather a work in progress that still needs a fair amount of progress.

Phonegap plugin for reading ambient noise level through microphone.



Supported platforms
-------------------
Android

iOS


Using
-----
Add to your build flow :
  cordova plugin add https://github.com/h1k3/micVolume.git


    micVolume.start(succesCallback, errorCallback);

   micVolume.read(function(reading){
        console.log(reading.volume);
    }, errorCallback);

    micVolume.stop(succesCallback, errorCallback);

In all cases, errorCallback passes back either an error message string or object with an error message string in it.
