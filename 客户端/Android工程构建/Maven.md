#Maven(咩ven)仓库介绍
- 软件仓库：存放可用软件包的服务  
 1. java/kotlin    __maven__
 2. IOS(objective-c/swift)  __cocoapods__
 3. node.js   __NPM__
 4.python __PyPI__
 5. php __PECL,Packaglist__
 
 #####中央仓库：https://mvnrepository.com/
 
 #####技术栈 ： gradle + maven 远程仓库
 
 #####maven仓库格式
 - 存储格式：xml格式 + 存储构件
 - POM：项目对象模型，project object model，包含了项目的基本信息
 用于描述项目如何构建，声明项目依赖
 - 主构件：唯一一个，项目本身
 - 从构件：相关附属构件（如doc文档，source源码构件）