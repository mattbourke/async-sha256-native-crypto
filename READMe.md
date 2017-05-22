# async sha256 function, using native crypto

This package contains a async sha256 function using the native crypto API.
Calling this function with an 'await' requires the code to be within a async block, see the below examples.

## Installation

```bash
npm install --save async-sha256
```

## Usage

```js
import sha256 from './async-sha256';

sha256('matt').then(function(hash){
  console.log(hash);
});
```

#### Or:

```js
import sha256 from './async-sha256';

async function doSomething() {
  let hash = await sha256('matt');
	console.log(hash);
}
doSomething();

```

## Change log

### 0.9.0

- Pushed: first version

### 1.0.0

- Pushed: relocated file, fixed bug, this can be 1.0.
