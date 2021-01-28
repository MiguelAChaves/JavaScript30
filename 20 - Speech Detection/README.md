# 20 - Speech Detection
## Introduction
This application detect Speech on en/us.

![SpeechRecognition](https://res.cloudinary.com/saaec/image/upload/v1611810437/speech_t3vl0i.jpg)

## Notes
* Optimization

    In the implementation, we use map function twice and join function to refer us to transcrip variable.

    ```javascript
    const transcript = Array.from(e.results)
      .map(result => result[0])
      .map(result => result.transcript)
      .join('');
    ```
    This can be solved in a cleaner way if we refer directly to the position.

    ```javascript
    const transcript = event.results[0][0].transcript;
    ```

## Learn more
* [SpeechRecognition](https://developer.mozilla.org/en-US/docs/Web/API/SpeechRecognition) from MDN web docs *Mozilla*

## Credits
Forked from Wes Bos ([wesbos/JavaScript30](https://github.com/wesbos/JavaScript30)) repository.
> Reviewed and recoded by Miguel Angel Chaves :shipit: (*@miguelachaves*)