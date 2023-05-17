# NX - monorepo

## NX 프로젝트 설치
```bash
yarn create nx-workspace
```

> 설치 항목에서 `Integrated monorepo` -> `Next.js` 선택

<img src="https://github.com/bytrustu/monorepo-nx/assets/39726717/c88bfec0-af8c-4620-9a92-210acbf3277c" />

## library ui 생성
```bash
nx g @nx/react:library ui
```

<img src="https://github.com/bytrustu/monorepo-nx/assets/39726717/053dd6be-bde5-405b-8d1d-33fa7019ad85" />


## ui에 스토리북 추가
```bash
nx g @nx/react:storybook-configuration ui
```


## yarn berry 버전 설정

```bash
yarn set version berry
```


## yarn berry pnp .yarnrc.yml파일 변경
```yml
nodeLinker: pnp
```
```bash
yarn
```


## 스토리북 실행 이슈
<img src="https://github.com/bytrustu/monorepo-nx/assets/39726717/faf8f1cd-ff11-4cc9-9fe8-f2dc8e313c57" />

```bash
yarn add -D @nx/devkit
```
```bash
yarn add -D @storybook/react
```


### yarn berry pnp 를 설정한 경우 yarn nx 로 실행 합니다.
```bash
yarn nx storybook ui
```
```bash
yarn nx serve client
```
