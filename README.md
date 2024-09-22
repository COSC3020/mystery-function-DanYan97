# Mystery Function

What does the `mystery()` function in the following piece of code do? Add your
answer to this markdown file.

```javascript
function mystery(a) {
    if(a.length == 1) return a[0];
    var foo = mystery(a.slice(1, a.length))
    if(foo > a[0]) return foo;
    else return a[0];
}

//This function uses a recursive algorithm which finds the maximum number in an array,
//more specifically, the array length is first reduced to 1 by the recursive calling, the
//element a[0] is returned to the end of the original array, this element is then compare
//with the previous one, if current a[0] is smaller than previous one, the previous element
//will replace a[0], if current a[0] is bigger, the element will stay, and moving to the
//next comparsion untill reach to the first element from the original array. Finally, the
//maximum number is found.
```

