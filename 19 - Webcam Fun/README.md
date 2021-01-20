# 19 - Webcam Fun
## Introduction
This application simulates a custom video player as like Youtube.

![Webcam](https://res.cloudinary.com/saaec/image/upload/v1611174726/webcam_nxezcd.jpg)

## Functionality
* Take photo -> Takes a photo from webcam device.
* RGB Sliders -> Changes RGB values with the apropiate effect.
## Notes
* Depreciation 

    The following has been depreceated by major browsers as of Chrome and Firefox.

    ```javascript
    video.src = window.URL.createObjectURL(localMediaStream);
    ```

    Please refer to these:
    Deprecated  - https://developer.mozilla.org/en-US/docs/Web/API/URL/createObjectURL
    Newer Syntax - https://developer.mozilla.org/en-US/docs/Web/API/HTMLMediaElement/srcObject

## Learn more
* [MediaDevices.getUserMedia()](https://developer.mozilla.org/es/docs/Web/API/MediaDevices/getUserMedia) from MDN web docs *Mozilla*
* [Media Capture and Streams API (Media Stream)](https://developer.mozilla.org/en-US/docs/Web/API/Media_Streams_API) from MDN web docs *Mozilla*
* [<a> Element](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/a) from MDN web docs *Mozilla*

## Credits
Forked from Wes Bos ([wesbos/JavaScript30](https://github.com/wesbos/JavaScript30)) repository.
> Reviewed and recoded by Miguel Angel Chaves :shipit: (*@miguelachaves*)
