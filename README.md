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
