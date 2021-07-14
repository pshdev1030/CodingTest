for in과 for of차이
https://jsdev.kr/t/for-in-vs-for-of/2938

set?

map?
has set get

from split
https://itskeleton.tistory.com/entry/Javascript-%EB%AC%B8%EC%9E%90%EC%97%B4-%EB%B0%B0%EC%97%B4%EB%A7%8C%EB%93%A4%EA%B8%B0-%EB%B0%B0%EC%97%B4-%EB%B6%84%ED%95%A0%EB%B3%80%ED%99%98%ED%95%98%EA%B8%B0-from


null과 undefined
https://medium.com/crocusenergy/js-undefined-null-어떨-때-쓸까-8782dc3c35b6

https://velog.io/@modolee/javascript-eval-is-evil

https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global_Objects/eval

NAN에 관하여
https://m.blog.naver.com/PostView.naver?blogId=ksh81850&logNo=220308841763&proxyReferer=https:%2F%2Fwww.google.com%2F

상속

객체의 복사
https://velog.io/@th0566/Javascript-%EC%96%95%EC%9D%80-%EB%B3%B5%EC%82%AC-%EA%B9%8A%EC%9D%80-%EB%B3%B5%EC%82%AC

https://medium.com/watcha/%EA%B9%8A%EC%9D%80-%EB%B3%B5%EC%82%AC%EC%99%80-%EC%96%95%EC%9D%80-%EB%B3%B5%EC%82%AC%EC%97%90-%EB%8C%80%ED%95%9C-%EC%8B%AC%EB%8F%84%EC%9E%88%EB%8A%94-%EC%9D%B4%EC%95%BC%EA%B8%B0-2f7d797e008a

prototype

진법 표현
toString(n)  
n진법에 해당하는 숫자로 변환된다.

문자열 뒤집기
n.split('').reverse().join('');  
뒤집어진다.

indexof,findIndex,find차이
https://humahumahuma.tistory.com/81

indexOf:배열에서 해당 값의 인덱스를 반환
```javascript
const superheroes = ['아이언맨', '캡틴 아메리카', '토르', '닥터 스트레인지'];

const index = superheroes.indexOf('토르');
console.log(index);
///2
```

findIndex:배열의 내용물이 객체일 때 해당 객체의 값으로 검색
```javascript
const todos = [
  {
    id : 1,
    text : '빨래',
    done: true
  },
  {
    id: 2,
    text: '숙제',
    done: true
  },
  {
    id : 3,
    text: '개밥주기',
    done: false
  }
];

const index2 = todos.findIndex(todo => todo.id === 1);
console.log(index2);
// 0
```

find 주어진 조건에 해당하는 내용물을 통쨰로 반환한다.
```javascript
const todos = [
  {
    id : 1,
    text : '빨래',
    done: true
  },
  {
    id: 2,
    text: '숙제',
    done: true
  },
  {
    id : 3,
    text: '개밥주기',
    done: false
  }
];

const index2 = todos.findIndex(todo => todo.id === 1);
console.log(index2);
// Object{id:1,text:'빨래',done:true}
```