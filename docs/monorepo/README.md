# 使用 monorepo 管理代码的方式

## lerna 的学习

## 安装

全局安装

```Shell
npm i -g lerna

# yarn
yarn global add lerna
```

## 理解 lerna

:::tip
我们要知道 lerna 有自己的工作流，learn 就是一个 monorepo 的脚手架工具，我们使用脚手架提供的能力就可以了。
:::

### 初始化一个 lerna 项目

```Shell
learn init
```

我们会得到一个 mono 管理的项目：
:::details
```json
// package.json
{
  "name": "root",
  "private": true, // 私有的，不会被发布，是管理整个项目，与要发布到npm的解耦
  "devDependencies": {
    "lerna": "^3.15.0"
  }
}
```

```js
// lerna.json
{
  "packages": [
    "packages/*"
  ],
  "version": "0.0.0"
}
```
:::