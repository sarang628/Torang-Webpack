https://webpack.js.org/guides/getting-started/

```
npm init -y
npm install webpack webpack-cli --save-dev
```

2개의 파일과 1개의 폴더가 생성됬다.
[package.json](package.json)
[package-lock.json](package-lock.json)
[node_modules](node_modules)

```
  webpack-demo
  |- package.json
  |- package-lock.json
 |- index.html
 |- /src
   |- index.js
```

index.js와 index.html 파일을 만들어준다.
```
function component() {
  const element = document.createElement('div');

  // Lodash, currently included via a script, is required for this line to work
  element.innerHTML = _.join(['Hello', 'webpack'], ' ');

  return element;
}

document.body.appendChild(component());
```

```
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8" />
    <title>Getting Started</title>
    <script src="https://unpkg.com/lodash@4.17.20"></script>
  </head>
  <body>
    <script src="./src/index.js"></script>
  </body>
</html>
```

이 상태에서 index.html 파일을 열면 코딩을 할 수 있다.