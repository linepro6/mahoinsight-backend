# MahoMaho INSIGHT!!
这里是**公主连结 Re:Dive 简体中文服**资讯站 [MahoMaho INSIGHT!! 真步真步视界术](https://mahomaho-insight.info) 后端工程的代码仓库。

## 技术栈
- [Node.js](https://nodejs.org/zh-cn/)
- [Koa.js](https://github.com/koajs/koa/)

## 项目构建与使用
### 项目环境准备
1.安装[Node.js](https://nodejs.org/zh-cn/) (版本要求14或更高)

2.使用以下命令安装nrm (可选)
```
npm install -g nrm
```
3.修改包管理器的下载源为淘宝镜像或cnpm (可选)
```
nrm use taobao
或
nrm use cnpm
```
4.使用以下命令安装[yarn](https://classic.yarnpkg.com/zh-Hans/)
```
npm install -g yarn
```
5.确保操作系统中已经安装过C++运行时或开发者工具。

### 项目依赖包的安装
```
yarn install
```

### 启动本地开发服务器
```
yarn start
```

### 更新前端文件缓存
```
yarn updatecache
```

### 项目本地环境参数配置
建议参考[Demo](https://github.com/nayurin/mahoinsight-backend/blob/master/.local_config.demo)进行配置，配置文件名为/.local_config.json
* port：服务端口
* address：服务器地址
* issuesroot：Issue的本地根路径，建议使用绝对路径
* cacheroot： 前端文件缓存的路径，建议使用绝对路径
* logroot: 日志文件保存的路径，可选配置，默认值为后端工程根目录/logs
* db：数据库文件路径，建议使用绝对路径

## 项目协作
### Issue
- 可以在项目Issues列表中[新建Issue](https://github.com/nayurin/mahoinsight-backend/issues/new)

### 贡献代码和PR
- 请```fork```本仓库到您的个人空间。如果本仓库代码更新了，同样需要同步最新修订到本地
  * 将本仓库的远程分支追加为fork仓库的上游：```git remote add upstream https://github.com/nayurin/mahoinsight-backend.git```
  * 同步上游的修订：```git fetch upstream```
  * 如果和本地内容出现冲突，需要在本地解决冲突
- 如果需要在新的分支上来调试代码，请使用```git checkout -b {分支名}```来创建新的分支
- ```{分支名}```请避免使用无意义的名字
  * 如果这是单模块内部的功能优化，建议使用```{模块名或接口名}-{优化内容}```来命名分支
  * 如果这是新功能的开发或是跨模块的功能优化，建议使用```feature-{特性名}```来命名分支
  * 如果这是对现存Bug的修复，则建议使用```fix-{bug名}```来命名分支
- 合并上游的修订：```git merge upstream/master```
- 在提交之前请仔细检查提交记录，尽量避免将个人环境的调试用代码提交到新分支。之后请使用```git push --set-upstream origin {您的本地分支名}```将本地分支推送到代码仓库的远程分支
- 每次提交PR之前**强烈建议**同步远端的仓库，以免遇到合并冲突的困扰
- 最后，请移步至代码仓库的[Pull Request](https://github.com/nayurin/mahoinsight-backend/pulls)页创建新的PR请求，CR通过后新代码会合入主分支

## 许可
本项目使用 MIT 许可，详情请参考 [LICENSE](https://github.com/nayurin/mahoinsight-backend/blob/master/LICENSE)