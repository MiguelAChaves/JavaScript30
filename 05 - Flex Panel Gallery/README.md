# 05 - Flex Panel Gallery
## Introduction
This application modifies spacing, blur and border color of a :framed_picture:

![Drum Kit](https://res.cloudinary.com/saaec/image/upload/v1609788569/CSS_Variables_hdiyue.jpg)

## Functionality
Inputs
* Frame spacing - slider
* Blur - slider
* Border color - color picker

## Notes
* Optimization
    
    Wes Bos purposes these code to trigger the function that modifies the attributes previously mentioned:

    ```javascript
    inputs.forEach(input => input.addEventListener('change', handleUpdate));
    inputs.forEach(input => input.addEventListener('mousemove', handleUpdate));
    ```
    As can be seen, with 'change' and 'mousemove', the action is triggered in two moments, however, we can make it efficient if we directly use the 'input' option, it will perform the same actions and in a single line of code.

    ```javascript
    inputs.forEach(input => input.addEventListener('input', handleUpdate));
    ```

## Learn more
* [Using CSS custom properties](https://developer.mozilla.org/es/docs/Web/CSS/Using_CSS_custom_properties) from MDN web docs *Mozilla*
* [HTMLElement.dataset](https://developer.mozilla.org/es/docs/Web/API/HTMLElement/dataset) from MDN web docs *Mozilla*

## Credits
Forked from Wes Bos ([wesbos/JavaScript30](https://github.com/wesbos/JavaScript30)) repository.
> Reviewed and recoded by Miguel Angel Chaves :shipit: (*@miguelachaves*)