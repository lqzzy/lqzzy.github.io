## 首次尝试

首先使用如下命令创建项目：

```plaintext
hexo init {name}
```

接下来我们首先进入新生成的文件夹里面，然后调用 Hexo 的 generate 命令，将 Hexo 编译生成 HTML 代码，命令如下：

```plaintext
hexo generate
```

可以看到输出结果里面包含了 js、css、font 等内容，并发现他们都处在了项目根目录下的 public 文件夹下面了。

然后我们利用 Hexo 提供的 serve 命令把博客在本地运行起来，命令如下：

```plaintext
hexo serve
```

部署命令如下：

```plaintext
npm install hexo-deployer-git --save
hexo deploy
```

## 主题

```plaintext
git clone [url] themes/[name]
```

## 文章

比如我们要新建一篇「HelloWorld」的文章，命令如下：

```sh
hexo new hello-world
```

在文件中categories属性后添加需要的分类，一篇文章可以有多个分类

## 部署

首先执行
```sh
chmod +x ./deploy.sh
```

然后执行
```sh
./deploy.sh
```
可以一键部署


## 数学

使用 `mathjax`, 需要额外安装插件

```sh
npm un hexo-renderer-marked --save
npm i hexo-renderer-kramed --save
```

## 插件

```sh
npm install hexo-auto-category --save
```
