# cntstr

A tiny utility to count the number of characters in a string.

## 📦 Installation

```bash
npm install cntstr
```

or with Yarn:

```bash
yarn add cntstr
```

## 🚀 Usage

### JavaScript（CommonJS）

```js
const { countCharacters } = require('cntstr');

const str = 'hello';
console.log(str); // Output: 5
```

### TypeScript（ESModule）

```ts
import { countCharacters } from 'cntstr';

const str: string = 'hello';
console.log(str); // Output: 5
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
