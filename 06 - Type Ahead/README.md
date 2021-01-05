# 06 - Type Ahead
## Introduction
This application filter a list of United States Cities and States:

![Cities](https://res.cloudinary.com/saaec/image/upload/v1609869999/fetch_qb2blt.jpg)

## Functionality
Type a City, State ...
![Cities](https://res.cloudinary.com/saaec/image/upload/v1609869999/fetch-typed_gnykuj.jpg)
## Notes
* Optimization
    
    Like the exercise three, the author purposes these code to trigger the function that modifies the attributes previously mentioned:

    ```javascript
    searchInput.addEventListener('change', displayMatches);
    searchInput.addEventListener('keyup', displayMatches);
    ```
    As can be seen, with 'change' and 'keyup', the action is triggered in two moments, however, we can make it efficient if we directly use the 'input' option, it will perform the same actions and in a single line of code.

    ```javascript
    searchInput.addEventListener('input', displayMatches);
    ```

## Learn more
* [FETCH API](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API) from MDN web docs *Mozilla*
* [Using Fetch](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API/Using_Fetch) from MDN web docs *Mozilla*

## Credits
Forked from Wes Bos ([wesbos/JavaScript30](https://github.com/wesbos/JavaScript30)) repository.
> Reviewed and recoded by Miguel Angel Chaves :shipit: (*@miguelachaves*)

