# cntstr

A tiny utility to count the number of characters in a string.

## 📦 Installation

```bash
npm install count-characters
```

or with Yarn:

```bash
yarn add count-characters
```

## 🚀 Usage

### JavaScript

```js
const { countCharacters } = require('cntstr');

console.log(countCharacters('hello')); // Output: 5
```

### TypeScript

```ts
import { countCharacters } from 'cntstr';

console.log(countCharacters('こんにちは')); // Output: 5
```

## 🧠 Function

```ts
export const countCharacters = (str: string): number => {
  return str.length;
};
```

- Takes a string as input
- Returns the total number of characters
- Works with multibyte characters as counted by `.length`

> ❗ **Note**: This function uses JavaScript's built-in `.length` method, which may not accurately count complex characters like emoji (👨‍👩‍👧‍👦). For full Unicode-aware counting, consider using [`grapheme-splitter`](https://www.npmjs.com/package/grapheme-splitter).

## 📄 License

MIT
