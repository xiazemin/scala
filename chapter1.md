# 安装

Mac OS X 和 Linux 上安装 Scala

第一步：Java 设置

确保你本地以及安装了 JDK 1.5 以上版本，并且设置了 JAVA\_HOME 环境变量及 JDK 的bin目录。

我们可以使用以下命令查看是否安装了 Java：

$ java -version

java version "1.8.0\_31"

Java\(TM\) SE Runtime Environment \(build 1.8.0\_31-b13\)

Java HotSpot\(TM\) 64-Bit Server VM \(build 25.31-b07, mixed mode\)

$

接着，我们可以查看是否安装了 Java 编译器。输入以下命令查看：

$ javac -version

javac 1.8.0\_31

$

如果还为安装，可以参考我们的Java 开发环境配置。

接下来，我们可以从 Scala 官网地址 http://www.scala-lang.org/downloads 下载 Scala 二进制包，本教程我们将下载 2.11.7版本，如下图所示：



解压缩文件包，可将其移动至/usr/local/share下：

mv scala-2.11.7 scala                   \# 重命名 Scala 目录

mv /download/scalapath /usr/local/share \# 下载目录需要按你实际的下载路径

修改环境变量，如果不是管理员可使用 sudo 进入管理员权限，修改配置文件profile:

vim /etc/profile



或



sudo vim /etc/profile

在文件的末尾加入:

export PATH="$PATH:/usr/local/share/scala/bin"

:wq!保存退出，重启终端，执行 scala 命令，输出以下信息，表示安装成功：

$ scala

Welcome to Scala version 2.11.7 \(Java HotSpot\(TM\) 64-Bit Server VM, Java 1.8.0\_31\).

Type in expressions to have them evaluated.

Type :help for more information.



