# CodeWars JS Solutions

---

## To square(root) or not to square(root)


Write a method, that will get an integer array as parameter and will process every number from this array.

Return a new array with processing every number of the input-array like this:

If the number has an integer square root, take this, otherwise square the number.

Example
[4,3,9,7,2,1] -> [2,9,3,49,4,1]
Notes
The input array will always contain only positive numbers, and will never be empty or null.

---

### Given Code


```js
function squareOrSquareRoot(array) {
  return array;  
}
```

---

### My Solution 


```js
function squareOrSquareRoot(array) 
{
      let newarr = [];
      for (var i = 0; i < array.length; i++) 
      {
        if (Number.isInteger(Math.sqrt(array[i])))
        {
          newarr.push(Math.sqrt(array[i]));
        }
        else
        {
          newarr.push(array[i]*array[i]);
        }
      }
        return newarr;
}
```


---

