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
