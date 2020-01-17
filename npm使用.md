### npm使用

npm config ls      查看npm配置

更改npm全局模块和cache的默认路径

npm  config set prefix "D:\npm\node_global_modules"
npm  config set cache "D:\npm\node_cache"


配置path环境变量：

D:\npm\node_global_modules

D:\npm\node_global_modules\node_modules

注意此处node_global_modules不能用node_modules为名字。



从cnpm下载有时会有错误(缺少某些依赖的模块)，此时从npm下载



大多数项目，webpack官方建议本地安装

