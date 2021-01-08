# 11 - Custom Video Player
## Introduction
This application simulates a custom video player as like Youtube.

![Cities](https://res.cloudinary.com/saaec/image/upload/v1610130423/video_player_po24gz.png)

## Functionality
* Play / Pause
* Volume slider
* Reproduction velocity slider
* Skip +25 / -10 seconds
## Notes
* Optimization
    
    Like others exercises, the author purposes these code to trigger the function that modifies the attributes previously mentioned:

    ```javascript
    ranges.forEach( range => range.addEventListener('change', handleRangeUpdate));
    ranges.forEach( range => range.addEventListener('mousemove', handleRangeUpdate));
    ```
    As can be seen, with 'change' and 'mousemove', the action is triggered in two moments, however, we can make it efficient if we directly use the 'input' option, it will perform the same actions and in a single line of code.

    ```javascript
    ranges.forEach( range => range.addEventListener('input', handleRangeUpdate));
    ```

## Learn more
* [Video and audio content](https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Video_and_audio_content) from MDN web docs *Mozilla*

## Credits
Forked from Wes Bos ([wesbos/JavaScript30](https://github.com/wesbos/JavaScript30)) repository.
> Reviewed and recoded by Miguel Angel Chaves :shipit: (*@miguelachaves*)
