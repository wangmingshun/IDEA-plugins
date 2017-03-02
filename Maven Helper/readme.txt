	我一般用这款插件来查看maven的依赖树。在不使用此插件的情况下，要想查看maven的依赖树就要使用Maven命令maven dependency:tree来查看依赖。
想要查看是否有依赖冲突也可以使用mvn dependency:tree -Dverbose -Dincludes=<groupId>:<artifactId>只查看关心的jar包，但是这样还是需要我执行命令，
并且当项目比较复杂的时候，这个过程是比较漫长的。maven helper就能很好的解决这个问题。

	一旦安装了Maven Helper插件，只要打开pom文件，就可以打开该pom文件的Dependency Analyzer视图（在文件打开之后，文件下面会多出这样一个tab），
进入Dependency Analyzer视图之后有三个查看选项，分别是Conflicts(冲突)、All Dependencies as List(列表形式查看所有依赖)、
All Dependencies as Tree(树结构查看所有依赖)。并且这个页面还支持搜索。很方便！并且使用该插件还能快速的执行maven命令。

插件地址：https://plugins.jetbrains.com/idea/plugin/7179-maven-helper