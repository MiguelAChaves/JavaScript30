
# 01 - JS and CSS Clock
## Introduction
This application simulates a ordinary clock with hands.

![Clock](https://res.cloudinary.com/saaec/image/upload/v1609783706/clock_bpyqqs.jpg)

## Notes
* Hand bug

    A small problem presented by the original code is that when a second, minute or hour hand matches 0, it turns into a unexpected behavior.

    From a Youtube user (*Quetin MCKay*), said one way to fix this bug: when seconds is 0, we need to remove the transition property, otherwise set it to normal (0.5s).

    ```javascript
    [secondHand, minHand, hourHand].forEach(
        handElement => handElement.style.transition = (seconds === 0) ? 'none' : null
    );
    ```


## Learn more
* [CSS Transform](https://www.w3schools.com/cssref/css3_pr_transform.asp) from W3 School
* [CSS Transition](https://www.w3schools.com/css/css3_transitions.asp) from W3 School

## Credits
Forked from Wes Bos ([wesbos/JavaScript30](https://github.com/wesbos/JavaScript30)) repository.
> Reviewed and recoded by Miguel Angel Chaves :shipit: (*@miguelachaves*)

