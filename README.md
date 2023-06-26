# JS Output Questions
Javascript  MCQ 
To flatten an array in JavaScript without using the `flat()` method, you can use a recursive function. Here's an example of how you can do it:

```javascript
let flat = [1, [2, 3, 4], 3];

function flattenArray(arr) {
  let result = [];

  arr.forEach((item) => {
    if (Array.isArray(item)) {
      result = result.concat(flattenArray(item));
    } else {
      result.push(item);
    }
  });

  return result;
}

let flattened = flattenArray(flat);
console.log(flattened);
```

Output:
```
[1, 2, 3, 4, 3]
```

In this code, the `flattenArray()` function takes an array as input and iterates over each element. If an element is an array, it recursively calls the `flattenArray()` function on that sub-array and concatenates the result with the current `result` array. If an element is not an array, it simply pushes it to the `result` array. Finally, the function returns the flattened array.

      const promise1 = new Promise((resolve, reject) => {
          resolve("3")
       })
       console.log('start')
       setTimeout(() => {
       console.log('setTimeout')
       })
       promise1.then((res) => {
       console.log(res);
       })
       console.log('end')

Output - start
end
3
setTimeout


            let a = 1;
             var b = 2;
            var test = function(){
             if (a === 1) {
             let i = 10;
             var j = 20;

             console.log(i)
             }
              console.log(i + 10)
             console.log(j + 1)
             console.log(a)
             console.log(b)
             }
             test()
             console.log(j)
            console.log("Welcome to Programiz!");

Output - 10
ERROR!  console.log(i + 10)
ReferenceError: i is not defined


            let a = 1;
             var b = 2;
            var test = function(){
             if (a === 1) {
             let i = 10;
             var j = 20;

             console.log(i)
             }
             console.log(j + 1)
             console.log(a)
             console.log(b)
             }
             test()
             console.log(j)
            console.log("Welcome to Programiz!");

Output - 10
21
1
2
ERROR!
 console.log(j)
ReferenceError: j is not defined

Write a code so that arr.print() must return 1,2,3,4 in JS

            // Add the print method to the Array prototype
            Array.prototype.print = function() {
              // Join the elements of the array with commas
              var result = this.join(',');
              console.log(result);
            };

            const arr = [1, 2, 3, 4];

            arr.print(); 
 // Output: 1,2,3,4

            console.log(x);
            var x=3;
            console.log(y);
            const y= 5;
            console.log(z);
            let z=8;

undefined
RE

            let abc = ()=>{
                console.log(this);
            }
            abc();

Output-{}

            function abc() {
                console.log(this);
            }
            abc();

Output - object [global]

            function foo() {
            let x= ( y=0)
            x++;
            y++;
            return x;
            }
            console.log(foo());

Output -1

            function foo(a,b,...c) {
                console.log(c);
            }
            foo(1,2,3,4,5);
             foo(1,2);
            
Output- [3,4,5]
[]

            const [a,...b,c]= [1,2,3,4;]
            console.log(a,b,c);
            
Output - ErrorRest element must be the last element

            (function x(){
                var a=b=5;
            })();
            console.log(a);
ReferenceError: a is not defined

            let a=[];
            let b=[];
            console.log(a==b);
            console.log(a===b);

Output - false
false

            let a=[];
            let b=a;
            console.log(a==b);
            console.log(a===b);

Output - true
true

            let a=[1,2,3,4]
            let b ={name:"san"}
            consol.log(...a)
output-1,2,3,4

            let a= 20 - - 30
            consolg.log(a);
Output - 40

            let a={nam: " sanya"}
            console.log(delete a.nam);
Output- true

            let a={nam: " sanya"}
            console.log(delete a);
Output- false // we can't delete object we can only delete its ppties

            const a =["san", "kas", "tan"];
            const [b]= a;
            console.log(a);
Output - san

How to get ppty without . operator
             const data={name:"san", age:24};
             const {name} = data;
             console.log(name)
 Output - san

             obj1={a:10};
             const obj2=obj1;
             obj1.a=20;
             console.log(obj1,obj2);
             let obj1;
Output- ReferenceError: Cannot access 'obj1' before initialization

             obj1={a:10};
             const obj2=obj1;
             obj1.a=20;
             console.log(obj1,obj2);
             var obj1;
Output -{ a: 20 }  { a: 20 }
