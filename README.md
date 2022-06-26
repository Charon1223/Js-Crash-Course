# Js-Crash-Course 

***
### 깃허브에 업로드 하는게 어언 세달이나 지났다. 그동안 개발 공부를 안한건 아니었지만 딱히 완성되는 프로젝트가 없었다. 
### 3개월 전 그 열정은 어디가고..
### html과 css는 간간히 하면서 이제 자바스크립트를 공부하려 한다
### 사실 모개발자 분의 바닐라 자바스크립트 챌린지도 진행했었는데 왠걸...너무 어렵고 진도를 따라가기 쉽지않아서 포기하였다.
### 하지만 포기는 배추세는 단위일뿐 나에게는 해당되지 않는다.
### 아무튼 오늘 유튜브에서 공부한 JS 속성 코스에서 공부한 내용을 적어보겠다.

***

## Array - 배열 ([] 대괄호에 목록을 넣는다)

```
const fruits = ['apples', 'oranges', 'pears'];

console.log(fruits);
->### apples, oranges, pears가 출력됨

그 외 
### fruits.**push**('mangos') -> 망고 추가
### fruits.**unshisft**('mangos') -> 망고를 맨 처음 위치
```

---
## Object 

```
const person = {
  firstName: 'John',
  lastName: 'Doe',
  age: 30,
  hobbies: ['music', 'movies', 'sports'],
  address: {
    street: '50 main st',
    city: 'Boston',
    state: 'MA'
  }
};


const { firstName, lastName, address: { city }} = person;

console.log(city);
->### Boston이 출력된다 
---


const todos = [
  {
    id: 1,
    text: 'Take out trash',
    isCompleted: true
  },
  {
    id: 2,
    text: 'Meeting with boss',
    isCompleted: true
  },
  {
    id: 3,
    text: 'Dentist appt',
    isCompleted: false
  },
];


const todoJSON = JSON.stringify(todos);
-> ### JSON 이라고 서버에 데이터로 보내는 방법이라 한다(사실 아직 잘모르겠다.. 아마도 백엔드에서 쓰는게 아닐지..)
```
### 일단 지금은 새벽2시니 여기까지만 하고
### 내일 나머지 공부해야겠다.


-----------
-----------

### 오늘 이어서 시작!

```

const todos = [
  {
    id: 1,
    text: 'Take out trash',
    isCompleted: true
  },
  {
    id: 2,
    text: 'Meeting with boss',
    isCompleted: true
  },
  {
    id: 3,
    text: 'Dentist appt',
    isCompleted: false
  },
];


// forEach, map, filter //
const todoCompleted = todos.filter(function(todo) {
  return todo.isCompleted === true;     __->위 3 id 중 isCompleted 값이 True인 항목만 출력__
}).map(function(todo) {
  return todo.text;          __-> 그 중 Text만 출력__
})
; 

console.log(todoCompleted);

```

---
##Switch (조건문/ ? / :)
```
const x = 9;

const color = x > 10 ? 'red' : 'blue'; __-> x가 10보다 작을때(?) true면 red, false면 blue/__

switch(color) {
  case 'red':
    console.log('color is red');
    break;
  case 'blue':
    console.log('color is blue');
    break;
  default:
    console.log('color is NOT red or blue');
    break;
} 
```
### 아...도통 머리에 들어오지 않는다..그냥 따라치기만 하는 수준인데 어떻게 해야 할까?

