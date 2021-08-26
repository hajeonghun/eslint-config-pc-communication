# PC-COMMUNICATION Javascript Coding Conventions
- eslint-config-pc-communication 는 자바스크립트 및 리액트 코딩컨벤션을 지원하는 [eslint](http://eslint.org/) 룰 셋입니다.
- eslint-config-pc-communication 는 [eslint-config-airbnb-base](https://github.com/airbnb/javascript/tree/master/packages/eslint-config-airbnb-base) 룰셋 기준으로 작성되었습니다.

> ### eslint-config-pc-communication는 2개의 룰 셋을 제공합니다.
> - ES6+ 룰 셋 : `pc-communication`
> - ES5 룰 셋 : `pc-communication/es5`

## Install
```
#npx install-peerdeps --dev eslint-config-pc-communication
```

## Usage
### ES6+ 룰 셋을 사용하는 경우
```
// .eslintrc 파일
{
  "extends": "pc-communication",
  "rules": {
    // 프로젝트별 적용할 Rules
  }
}
```

### ES6+ 와 React hooks(requires v16.8+)를 사용하는 경우
```
// .eslintrc 파일
{
  "extends": ["pc-communication", "pc-communication/hooks"],
  "rules": {
    // 프로젝트별 적용할 Rules
  }
}
```

### ES5 룰 셋을 사용하는 경우
```
// .eslintrc 파일
{
  "extends": "pc-communication/es5",
  "rules": {
    // 프로젝트별 적용할 Rules
  }
}
```

### ES5 와 React hooks(requires v16.8+)를 사용하는 경우
```
// .eslintrc 파일
{
  "extends": ["pc-communication/es5", "pc-communication/hooks"],
  "rules": {
    // 프로젝트별 적용할 Rules
  }
}
```

### Prettier 추가 
```
// .prettierrc 파일
{
  "singleQuote": true,
  "jsxSingleQuote": false,
  "semi": true,
  "useTabs": false,
  "tabWidth": 2,
  "trailingComma": "all",
  "printWidth": 80,
  "arrowParens": "avoid",
  "bracketSpacing": false
}
```

### Auto Formatting 관련 패키지 설치 및 적용
```
npm install --save-dev eslint-plugin-prettier eslint-config-prettier
```
```
// .eslintrc 파일
// js만 적용 시
extends: ['pc-communication', 'plugin:prettier/recommended'],

// js + react 적용 시
extends: ['pc-communication', 'pc-communication/hooks', 'plugin:prettier/recommended'],
```


## PC-COMMUNICATION JavaScript Style Guilde
상세한 내용은 다음의 JavaScript 스타일 가이드를 참조하세요  
### [PC-COMMUNICATION JavaScript Style Guilde](STYLE_GUIDE.md)

## PC-COMMUNICATION React Hooks Style Guide
상세한 내용은 다음의 JavaScript 스타일 가이드를 참조하세요
### [PC-COMMUNICATION React Hooks Style Guilde](REACT_STYLE_GUIDE.md)


## License
`eslint-config-pc-communication` is released under the [MIT license](LICENSE).

```
Copyright (c) 2021 PC-COMMUNICATION Corp.

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.  IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
```
