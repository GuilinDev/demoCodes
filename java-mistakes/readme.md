### 说明

- 所有代码基于Java 11 + Spring Boot 2.2.1.RELEASE + Spring Cloud Greenwich.SR4 + Spring Data Moore-SR4开发，基于Maven做依赖管理。
- 每一个案例都是独立的SpringBoot或Java命令行应用程序，可以单独启动，避免相互干扰，但是它们公用一个Maven POM。
- 下载源码后，先在根目录运行docker-compose up命令来通过Docker运行相关的MySQL、Redis、ES、RabbitMQ等系统，随后再来启动应用。
- 专栏大部分内容只依赖MySQL一个组件，如果docker-compose启动有困难的话可以先注释docker-compose.yml中的相关组件，比如注释ES和RabbitMQ，等后面设计篇需要用到的时候再启动，并且需要同时删除pom.xml中的相关SpringBoot Starter模块。
- 源码根目录下有一个readme.md的Markdown文件，这里有一个目录列了每一个主题对应的源码位置，同时来到每一个源码包中下面还有一个readme.md文件，里面列了每个主题中每一个小节的源码包名。
- 大多数源码中的案例都会使用wrong和right这样方法命名来代表错误实现和正确实现，可以结合文章对比实现来理解。
- 有一些案例（比如SQL索引一文）会基于当前时间生成测试数据，所以不确保文中的测试结果本地可以重现，需要调整测试用例。

