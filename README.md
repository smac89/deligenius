# dg.ts

> Lightweight Deno middleware framework 


### Features

* Light weight (11kb)
* Adapted from Koa and Express syntax
* Near deno http module performance
* Body parser middleware option
* Gentle error handling

### Quick Start Examples

##### Hello World example
1. Use your favourite editor, copy below to ```app.ts```
```ts
// ./app.ts
import { Application} from "https://raw.githubusercontent.com/deligenius/dg.ts/master/mod.ts";

let app = new Application({ port: 8000 }).listen();

app.use((ctx) => {
  ctx.send("Hello World!");
});
```
2. Run program with
```ts
> deno run --allow-net ./app.ts
```

##### Using router
If you write code in the ```express.js``` way, it's recommended to use ```Router```, as it comes with ```get```, ```post```, ```put```, ```delete``` ... methods

