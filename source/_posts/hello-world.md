---
title: Hello World Demo
date: 2022-02-15 22:56:02
---
Welcome to [Hexo](https://hexo.io/)! This is your very first post. Check [documentation](https://hexo.io/docs/) for more info. If you get any problems when using Hexo, you can find the answer in [troubleshooting](https://hexo.io/docs/troubleshooting.html) or you can ask me on [GitHub](https://github.com/hexojs/hexo/issues).

## Quick Start

### Create a new post

```js
// test.js
'use strict';

let times = 0;

function run() {
  let str = 'var a = "';
  for (let i = 0; i < 100 * 1024 / 18; i++) str += Math.random().toString();
  str += '";';

  const script = new (require('vm').Script)(str);
  times++;
  if (times % 1000 === 0) console.log(times);
}

(async () => {
  while (true) {
    run();

    await new Promise(resolve => {
      setTimeout(() => {
        resolve();
      }, 10);
    });

    gc();
  }
})();
```

``` bash
$ hexo new "My New Post"
```

More info: [Writing](https://hexo.io/docs/writing.html)

### Run server

``` bash
$ hexo server
```

More info: [Server](https://hexo.io/docs/server.html)

### Generate static files

``` bash
$ hexo generate
```

More info: [Generating](https://hexo.io/docs/generating.html)

### Deploy to remote sites

``` bash
$ hexo deploy
```

More info: [Deployment](https://hexo.io/docs/one-command-deployment.html)
