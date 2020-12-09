## 리액트가 만들어진 이유

리액트는 어떠한 상태가 바뀌었을때, 그 상태에 따라 DOM 을 어떻게 업데이트 할 지 규칙을 정하는 것이 아니라, 

아예 다 날려버리고 처음부터 모든걸 새로 만들어서 보여준다면 어떨까? 라는 아이디어에서 시작되었다.

![react](https://blog.kakaocdn.net/dn/eD2dhU/btqPC1vxyMK/KTQSTkirZMFrCQOCZN9a7K/img.gif)

그러면 "업데이트를 어떻게 해야 할 지"에 대한 고민을 전혀 안해도 되기 때문에 개발이 정말 쉬워질 것이다.

하지만, 정말로 동적인 UI 를 보여주기 윟서 모든걸 다 날려버리고 모든걸 새로 만들게 된다면, 속도가 굉장히 느릴것이다.

하지만, 리액트에서는 Virtual DOM 이라는 것을 사용해서 이를 가능케 했다.

리액트는 상태가 업데이트 되면, 업데이트가 필요한 곳의 UI 를 Virtual DOM 을 통해서 렌더링한다.

![react](https://blog.kakaocdn.net/dn/L6WLG/btqPFTQ4mJ5/e5hvhWvi33ZVlK3ouuKA31/img.png)

그리고 나서 리액트 개발팀이 만든 매우 효율적인 비교 알고리즘을 통하여 실제 브라우저에 보여지고 있는 DOM 과 비교를 한 후, 차이가 있는 곳을 감지하여 이를 실제 DOM 에 패치시켜준다. 이를 통하여, "업데이트를 어떻게 할 지" 에 대한 고민을 하지 않으면서, 빠른 성능도 지켜낼 수 있게 되었다.

---

## \- Node.js 설치하기

#### nvm (Node Version Manager)

: mac의 경우 nvm을 통해 설치하는게 좋음

[https://github.com/nvm-sh/nvm](https://github.com/nvm-sh/nvm)

```
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.37.0/install.sh | bash
```

\- curl 이용

```
nvm install --lts

```

\- node lts (Long Term Support) version 설치

: window의 경우 공식 홈페이지에서 설치

[nodejs.org/ko/download/](https://nodejs.org/ko/download/)

---

## \- Yarn 설치하기

[classic.yarnpkg.com/en/docs/install/#mac-stable](https://classic.yarnpkg.com/en/docs/install/#mac-stable)

```
brew install yarn
```

: mac

\- homebrew 이용 

: window

[classic.yarnpkg.com/en/docs/install/#windows-stable](https://classic.yarnpkg.com/en/docs/install/#windows-stable)

---

## \- React 설치 및 사용

[github.com/facebook/create-react-app](https://github.com/facebook/create-react-app)

```
npx create-react-app (folder name)
```

: npx

```
yarn create react-app (folder name)
```

: yarn

```
cd hello-react
yarn start
```

---

※ 출처

[react.vlpt.us/](https://react.vlpt.us/)
