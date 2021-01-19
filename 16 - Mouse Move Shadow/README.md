# 16 - Mouse Move Shadow
## Introduction
This application displays a text effect with mouse movement

![Text](https://res.cloudinary.com/saaec/image/upload/v1611010178/text_xvxyce.jpg)

## Notes
* Optimization

    In the implementation, we use the properties of the offsetX and offsetY to locate the cursor, the downside is that switching between parent and child element it changes respect to each.

    ```javascript
    let { offsetX: x, offsetY: y } = e;

    if (this !== e.target) {
      x = x + e.target.offsetLeft;
      y = y + e.target.offsetTop;
    }
    ```
    This can be solved in a cleaner way if we refer to the viewport, with the properties of clientX and clientY.

    ```javascript
    let { clientX: x, clientY: y } = e;
    ```

## Learn more
* [contenteditable](https://developer.mozilla.org/es/docs/Web/HTML/Atributos_Globales/contenteditable) from MDN web docs *Mozilla*
* [MouseEvent.clientX](https://developer.mozilla.org/en-US/docs/Web/API/MouseEvent/clientX) from MDN web docs *Mozilla*

## Credits
Forked from Wes Bos ([wesbos/JavaScript30](https://github.com/wesbos/JavaScript30)) repository.
> Reviewed and recoded by Miguel Angel Chaves :shipit: (*@miguelachaves*)
