# simple-ui

Simple common function in typescript to manage react project.

### Install

```bash
npm i @ndeuja/simple-ui
```

### Usage

```jsx
import {
  UpdateObject,
  UpdateArray,
  ShortArray,
  GetIndexBy,
  ShortNameGenerate,
} from "@ndeuja/simple-ui";

let OldObj = { name: "Nimesh Deuja" };
let UpdatedObj = UpdateObject(OldObj, { age: 32 });
// return {name: 'Nimesh Deuja', age: 32}

let OldArr = [{ name: "Nimesh Deuja", age: 32 }];
let UpdatedArr = UpdateArray(OldArr, {
  name: "Abhisekh Deuja",
  age: 34,
});
// return [{name: 'Nimesh Deuja', age: 32},{name: 'Abhisekh Deuja',age: 34}]

let ShortedArr = ShortArray(UpdatedArr, "ASC", "name");
// return [{name: 'Abhisekh Deoja',age: 34},{name: 'Nimesh Deuja', age: 32}]

let index = GetIndexBy(ShortedArr, 34, "age");
// return 0

let ShortName = ShortNameGenerate("Nimesh Deuja");
// return 'ND'

```

### Author

Nimesh Deuja
