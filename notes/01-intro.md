# 01 :: Intro

> Notes/Talking Points

- JavaScript syntactic superset; layers additional concepts on top to add types to JS (at compile time)
- Microsoft, so _of course_ it sucks. Like VSCode. And Outlook on iOS. And now GitHub.

Great example of usage/need considering the snippet:

```
const add = (a, b) => a + b;

const v1 = add(1, 1);
const v2 = add('hello', 'world');
const v3 = add(1, '1');

console.log(v1, typeof v1); // 2, number
console.log(v2, typeof v2); // 'helloworld', string
console.log(v3, typeof v3); // '11', string
```

in TS, intent is clear ...

```
const add: number = (a: number, b: number) => a + b;
...
add('1', 1); // console says, "QUIT IT!"
```

- predictable contracts in JavaScript?!
