# TypeScript

### TypeScript #1 타입스크립트를 쓰는 이유

JavaScript(동적언어) : 런타임에 타입 결정 / 오류 발견
Java, TypeScript(정적언어) : 컴파일 타임에 타입 결정 / 오류 발견

```ts
function add(num1: number, num2: number) {
  console.log(num1 + num2)
}

// add();
// add(1);
add(1, 2)
// add(3, 4, 5);
// add("hello", "world");
```

```ts
function showItems(arr:number[]) {
  arr.forEach((item) => {
    console.log)(item);
  });
}

showItems([1,2,3]);
// showItems(1,2,3);
```

### TypeScript #2 기본 타입

```ts
let car:string = 'bmw';
let age:number = 30;
let isAdult:boolean = true;
let a:number[] = [1,2,3];
let a2:Array<number> = [1,2,3];
let week1:string[] = ['mon', 'tue', 'wed'];
let week12:Array<string> = ['mon', 'tue', 'wed'];

- 튜플 (Tuple)

let b:[string, number];
b = ['z', 1];
// b= [1,'z'];
b[0].toLowerCase();
// b[1].toLowerCase();

-  void, never

function sayHello():void{
  console.log('hello');
}
function showError:never(){
  throw new Error();
}
function infLoop:never(){
  while (true) {
    // do something..
  }
}

- enum

enum OS {
  Window = 3,
  Ios = 10,
  Android

  양방향
}
console.log(Os[10]) // Ios
console.log(Os['Ios']) // 10

enum OS {
  Window = 'win',
  Ios = 'ios',
  Android = 'and'

  단방향
}

let myOs:Os;
myOs = Os.Window

특정 값만 입력할 수 있게 강제하고 싶을 때,
그리고 그 값들이 공통점이 있을 때 사용.

- null, undefined

lett a:null = null;
let b:undefined = undefined;

```
