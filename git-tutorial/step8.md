# Make your changes 2
Now that we are on our feature branch, we are going to change one of the functions in our `fibonacci.js` to use an iterative method, stage the changes and commit them to our feature-branch. Go ahead and open the file in the text editor.

As our change we'll simply replace the code with:

```js
function fib(num) {
  var n = parseInt(num);
  
  let arr = [0,1]
  
  var i;
  for (i = 2; i < (n + 2); i++ ) {
    arr.push(arr[i-1] + arr[i-2]);
  }

  return arr[n+1];
}

const num = process.argv.slice(2);

console.log(fib(num));

//Also, whoever wrote this is bad at coding
```
Click `bash shortcut.sh`{{execute}} to replace the text.

This changes the fibonacci from the, clearly inferior, recursive calculation to, instead, use dynamic programming. It's what the pros do. Recommended by 9 out of 10 dentists.

To check the status of our work so far, run the `git status`{{execute}} command.

Now you can stage the file by running the add command: `git add fibonacci.js`{{execute}}

#### Examples
Adds all changes files:

`git add --a`

Adds content from all *.txt files under Documentation directory and its subdirectories:

`git add Documentation/\*.txt`

Considers adding content from all git-*.sh scripts:

`git add git-*.sh`
