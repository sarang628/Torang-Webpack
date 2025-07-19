Swagger를 실행해보려고 가이드를 봤더니, webpack과 같은 도구를 통해 실행할 수 있는 것 같다.

webpack 사용법을 몰라 가이드를 따라가며 하나씩 실행해 보려고 한다.(Swagger 하나 바꾼다는게 할 게 끝이 없다..)

# getting-started

# 웹팩이란?

- static modular bundler 
  - html, css, javaScript, image 등을 하나 또는 여러개의 파일로 묶어주는 도구
  - 동적이 아닌 정적 static 이다. 웹이지만 컴파일을 해서 프로그램을 만들어야 한다.
- JavaScript application
- webpack은 javascript 모듈을 컴파일 하는데 사용

https://webpack.js.org/guides/getting-started/

webpack은 javascript 모듈을 컴파일 하는데 사용 된다.

설치하고 나면 CLI나 API를 통해 사용 한다.

새로운 사용자라면 [core concept](https://webpack.js.org/concepts/) 과 this comparion (https://webpack.js.org/comparison/) 을 읽어라.

다른 툴 보다 webpack을 사용해야 하는지 알 수 있다.

javascript modules 은 무엇?
core concept 페이지를 보다보니

Learn more about JavaScript modules and webpack modules [here](https://webpack.js.org/concepts/modules/)

을 찾을 수 있었다.


# Core concept

webpack은 static modular bundler 또는 JavaScript application 이다.

webpack이 application을 처리할 때, 내부적으로 하나 이상의 entry points에서 의존성 그래프를 빌드한다. 

그리고 프로젝트에서 필요한 모든 모듈을 bundles에 합쳐 넣는다.

bundles : 컨텐츠를 서비스 하기 위한 static assets


# Module

모듈을 이해하기위하선 [modular programming](https://en.wikipedia.org/wiki/Modular_programming) 라는 것을 알아야 한다. (ㅠㅠ)

대충 유추해보면 프로그램 하나에 모든 기능을 넣지말고 기능별로 잘 나누어 여러개의 프로그램을 나눠 실행하자는 의미로 이해하면 될 것 같다.

Webpack Module 란?

다양한 방법으로 모듈을 표현 가능

import, require(), define, require, @import, stylesheet url(...), HTML <img src=...> 같은 방법으로 모듈을 사용 할 수 있다는 것 같다.

An ES2015 import statement
A CommonJS require() statement
An AMD define and require statement
An @import statement inside of a css/sass/less file.
An image url in a stylesheet url(...) or HTML <img src=...> file.

