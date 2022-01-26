# Welcome to Remix!

- [Remix 文档](https://remix.run/docs)

## 开发

在终端中运行:

```sh
npm run dev
```

这个命令会以开发模式启动你的应用，当源文件修改时会自动重新构建。

## 部署

首先，以生产模式构建你的应用：

```sh
npm run build
```

然后以生产模式启动应用：

```sh
npm start
```

Now you'll need to pick a host to deploy it to.

### 自定义

如果你熟悉 node 应用部署，内置的 Remix 应用服务器是可以在生产环境使用的。

确保部署 `remix build` 命令执行的产物。

- `build/`
- `public/build/`

### 使用模版

当你运行 `npx create-remix@latest`，会有几种选择来任你挑选。你可以重新运行一次命令来创建一个新项目，然后把 `app/` 目录复制到一个为你的服务器预设的新项目。

```sh
cd ..
# 创建一个新项目, 选择一个事件配置好的主机
npx create-remix@latest
cd my-new-remix-app
# 删除新项目的app目录 (不是老项目!)
rm -rf app
# 复制 app 文件夹
cp -R ../my-old-remix-app/app app
```
