## readme 

1. 源文件分支为dev, 生成的部署分支为master
2. 不走github Action了，直接本地/bin/deploy，会自动更新master分支，并且push到github上
3. github会自动把master的内容同步到网站上

## 源地址

https://github.com/alshedivat/al-folio

## workflow流程

两种，第一种，通过在git项目中配置.github/**，然后github会在自己的服务器上编译和运行项目
完成整个的部署过程

第二种，不通过action，直接在本地生成master，然后推送上去，github无需编译，速度更快，内容也有保证