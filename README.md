# go1-coding-challenge
Respository of code challenges for Go1 technical interviews. 


## Coding Challenges

- [Learners and Courses](./learners-and-courses/learners-and-courses.md) [[data](./learners-and-courses/learners-and-courses.data.md)]

```js
const fn = (data) => {
    let s = {};
    for(let i in data){
        for(let j of data[i]){
            s[`${j}`] = s[`${j}`] >= 0 ? s[`${j}`] + 1 : 0;            
        }
    }
    return Object.keys(s).filter(item =>{ if(s[item] == 0) return item;})          
}
fn({
  "Learner-0001": [
    "Course-0001",
    "Course-0002",
    "Course-0003",
    "Course-0001",
    "Course-0002",
    "Course-0003",
  ],
  "Learner-0002": [
    "Course-0002",
    "Course-0003",
    "Course-0004"
  ]
});
```

- [Quiz Results](./quiz-results/quiz-results.md) [[data](./quiz-results/quiz-results.data.md)]
- [Watched Courses](./watched-courses/watched-courses.md) [[data](./watched-courses/watched-courses.data.md)]
- [Concurrent Learners](./concurrent-learners/concurrent-learners.md) [[data](./concurrent-learners/concurrent-learners.data.md)]

## Helpful Snippets

Quickly read in JSON with [these](json-import-examples.md) snippets in multiple languages.

## How to Create New Challenges

[This](HOWTO.md) file contains instructions for creating new challenges.

