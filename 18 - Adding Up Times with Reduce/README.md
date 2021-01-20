# 18 - Adding Up Times with Reduce
## Introduction
This practices show us how to use reduce properly.

## Notes
* Optimization

    In the implementation, to obtain the final number of seconds, two map functions and a reduce function are used.

    ```javascript
    const seconds = timeNodes
    .map(node => node.dataset.time)
    .map(timeCode => {
      const [mins, secs] = timeCode.split(':').map(parseFloat);
      return (mins * 60) + secs;
    })
    .reduce((total, vidSeconds) => total + vidSeconds);
    ```
    This can be solved in a cleaner way if we only use reduce once.

    ```javascript
    const seconds = timeNodes.reduce((total,currValue) => {
      const [mins, secs] = currValue.dataset.time.split(':');
      return total + (mins * 60) + (secs * 1);
    },0);
    ```
    
    The author proposes to calculate the hours, minutes and seconds doing math.

    ```javascript
    let secondsLeft = seconds;
    console.log(secondsLeft);
    const hours = Math.floor(secondsLeft / 3600);
    secondsLeft = secondsLeft % 3600;

    const mins = Math.floor(secondsLeft / 60);
    secondsLeft = secondsLeft % 60;

    console.log(hours, mins, secondsLeft);
    ```
    This can be solved in a cleaner way if we use Date() function and its own properties.

    ```javascript
    const measuredTime = new Date(seconds * 1000);
    console.log(measuredTime.getUTCHours() , measuredTime.getUTCMinutes() , measuredTime.getUTCSeconds());
    ```

## Learn more
* [Date](https://developer.mozilla.org/es/docs/Web/JavaScript/Referencia/Objetos_globales/Date) from MDN Web Docs.


## Credits
Forked from Wes Bos ([wesbos/JavaScript30](https://github.com/wesbos/JavaScript30)) repository.
> Reviewed and recoded by Miguel Angel Chaves :shipit: (*@miguelachaves*)
