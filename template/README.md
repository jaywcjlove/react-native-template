# React Native UIW Template

[![](https://img.shields.io/npm/v/@uiw/react-native-template.svg?color=success&style=flat-square)](https://www.npmjs.com/package/@uiw/react-native-template)
[![](https://img.shields.io/github/issues/uiwjs/react-native-template.svg?style=flat-square)](https://github.com/uiwjs/react-native-template/issues)
[![](https://img.shields.io/github/forks/uiwjs/react-native-template.svg?style=flat-square)](https://github.com/uiwjs/react-native-template/network)
[![](https://img.shields.io/github/stars/uiwjs/react-native-template.svg?style=flat-square)](https://github.com/uiwjs/react-native-template/stargazers)
[![](https://img.shields.io/github/release/uiwjs/react-native-template?style=flat-square)](https://uimjs.github.io/#/docs/react-native-template/releases)

[React Native](https://github.com/facebook/react-native) Template for [@uiw/react-native](https://github.com/uiwjs/react-native-uiw). 


> Migrate from @uiw/react-native-template 0.1.2 to [v1.1.0](https://github.com/uiwjs/react-native-template/releases/tag/v1.1.0)

## Features

This template includes the following:

- Elegant usage directly within the [React Native CLI](https://github.com/react-native-community/cli)
- [React Native](https://github.com/facebook/react-native) 0.60 support (now with Hooks! 🙌).
- Easy to use and understand folder structure to get you up and running as fast as possible.
- [@uiw/react-native](https://github.com/uiwjs/react-native-uiw) component framework and themes.
- Using [react-navigation](https://github.com/react-navigation/react-navigation) to routing and navigate your React Native applications.
- [Redux](https://github.com/reduxjs/redux) support (with [@rematch](https://github.com/rematch/rematch) example)
- [ESLint](https://github.com/eslint/eslint), and [Prettier](https://github.com/prettier/prettier) configured out-of-the-box
- Using [mocker-api](https://github.com/jaywcjlove/mocker-api) that creates mocks for REST APIs.

## Installation and Usage

🚧 This template only works with the new CLI. This template is intended for React Native versions `>= 0.61`. It has not been tested with previous versions. 

**Note on the legacy CLI**

🚧 There seems to be quite some confusion about the legacy CLI. This template only works with the new CLI. Make sure you have uninstalled the legacy `react-native-cli` first (`npm uninstall -g react-native-cli`), for the below command to work. 

```bash
npm uninstall -g react-native-cli
```

Further information can be found here: https://github.com/react-native-community/cli#about


### Macbook 安装
```bash
cd app/ios
$ bundle install
$ bundle exec pod install
```

Macbook **`M1`** 安装

```bash
cd app/ios
$ arch -arm64 bundle install
$ arch -arm64 bundle exec pod install
```

启动 React Native **ios** 服务

```bash
cd shared
$ yarn run api 
$ yarn run ios 
```

**`react-native@0.61.0` or higher**

```sh
npx react-native init MyApp --template @uiw/react-native-template
# npx react-native init MyApp --template @uiw/react-native-template@v1.0.0
```

**If you wish to not use `npx`**

you can also install the new CLI globally (`npm i -g @react-native-community/cli` or `yarn global add @react-native-community/cli`).

```bash
npx react-native init MyApp --template @uiw/react-native-template

cd MyApp/app/ios
# Installing CocoaPods dependencies
pod install 
```

```bash
# This will initialize new project using template from TEMPLATE_NAME package
npx react-native init ProjectName --template ${TEMPLATE_NAME}

# This will initialize new project using init command from react-native@VERSION
# but will use TEMPLATE_NAME custom template
npx react-native@${VERSION} init ProjectName --template ${TEMPLATE_NAME}
```
## @uiw/react-native-uiw文档本地预览
```bash
cd MyApp
$ yarn run doc
```

## Use husky

Edit package.json > prepare script and run it once:
```bash
cd MyApp/shared
npm pkg set scripts.prepare="husky install"
npm run prepare
```
Add a hook:
```bash
npx husky add .husky/pre-commit "npm run precommit"
git add .husky/pre-commit
```

Make a commit:
```bash
git commit -m "Keep calm and commit"
# `npm precommit` will run
```

## Dependencies

```bash
@react-navigation/native
  ├──react-native-gesture-handler
  ├──react-native-reanimated
  ├──react-native-screens
  ├──react-native-safe-area-context
  └──@react-native-community/masked-view
```

## 目录结构
```
.
├── .gitignore
├── README.md
├── app         # iOS/Android 原生应用
│   ├── android
│   ├── app.json
│   ├── index.js
│   ├── ios
│   ├── metro.config.js
│   ├── package.json
│   └── tsconfig.json
├── package.json
└── shared    # React Native 业务逻辑
    ├── README.md
    ├── package.json
    └── src
        └── App.js
```

## Links

- [React Native upgrade helper](https://react-native-community.github.io/upgrade-helper/)

## Contributors

As always, thanks to our amazing contributors!

<!--AUTO_GENERATED_PLEASE_DONT_DELETE_IT--><a href="https://github.com/jaywcjlove" title="小弟调调">
  <img src="https://avatars.githubusercontent.com/u/1680273?v=4" width="42;" alt="小弟调调"/>
</a>
<a href="https://github.com/renovate-bot" title="Mend Renovate">
  <img src="https://avatars.githubusercontent.com/u/25180681?v=4" width="42;" alt="Mend Renovate"/>
</a>
<a href="https://github.com/ChenlingasMx" title="Chenling">
  <img src="https://avatars.githubusercontent.com/u/59959718?v=4" width="42;" alt="Chenling"/>
</a>
<a href="https://github.com/cuilanxin" title="崔兰鑫">
  <img src="https://avatars.githubusercontent.com/u/57083007?v=4" width="42;" alt="崔兰鑫"/>
</a>
<a href="https://github.com/matuancc" title="cc">
  <img src="https://avatars.githubusercontent.com/u/33281802?v=4" width="42;" alt="cc"/>
</a>
<a href="https://github.com/Amber-Nan" title="Amber-Nan">
  <img src="https://avatars.githubusercontent.com/u/66067296?v=4" width="42;" alt="Amber-Nan"/>
</a>
<a href="https://github.com/panbibi" title="panbibi">
  <img src="https://avatars.githubusercontent.com/u/81728478?v=4" width="42;" alt="panbibi"/>
</a>
<a href="https://github.com/wwmmzz" title="...">
  <img src="https://avatars.githubusercontent.com/u/26562795?v=4" width="42;" alt="..."/>
</a>
<a href="https://github.com/xingyuefeng" title="xyf">
  <img src="https://avatars.githubusercontent.com/u/24369183?v=4" width="42;" alt="xyf"/>
</a>
<a href="https://github.com/SunLxy" title="逍遥">
  <img src="https://avatars.githubusercontent.com/u/49544090?v=4" width="42;" alt="逍遥"/>
</a><!--AUTO_GENERATED_PLEASE_DONT_DELETE_IT-END-->

Made with [contributors](https://github.com/jaywcjlove/github-action-contributors).


## License

This project is [MIT](LICENSE) licensed.
