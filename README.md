# M42kup

JavaScript로 M42kup의 HTML 렌더러를 구현한 것입니다. 아직 만들고 있음.\
M42kup이 뭔지는 어딘가에 쓸 예정입니다.\
테스트 페이지 제공 예정.

## 설치

```bash
~ $ git clone https://github.com/logico-philosophical/m42kup.git
~ $ cd m42kup
~/m42kup $ npm install
```

## 테스트
```bash
~/m42kup $ node
> m42kup = require('./index')
> m42kup.render('[*hi]')
'<span class="m42kup"><i>hi</i></span>'
```

## API (불안정)

### `m42kup.render(input)`

#### 입력
* `input`: M42kup 문법을 따르는 문자열.

#### 출력
HTML로 렌더링 된 것의 문자열이 출력됩니다. `<span class="m42kup">`이랑 `</span>`으로 감싸져 있음.

#### 입출력 예시
```bash
> m42kup.render('[*hi]')
'<span class="m42kup"><i>hi</i></span>'
