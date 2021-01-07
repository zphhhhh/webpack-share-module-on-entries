1. `npm i`
2. `npm run webpack`
3. open `http://localhost:8080/` 
4. open Chrome devtool see the `console`:

```
This is math.js!
index 3
This is math.js!
index2 3
```

We see `This is math.js!` twice, but i hope to see only once.

5. `npm run browser`
6. open Chrome devtool see the `console`:

```
This is math.js!
index 3
index2 3
```
### Why?

ES6 import is static, it is the same object no matter how many times it is imported.

But webpack makes it to be a new object every time it is imported be different entries.
