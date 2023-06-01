# JSOutputQuestions

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
