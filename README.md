 for java
java异常整理

java.lang.NullPointerException

    java.lang.NullPointerException

问题描述

    at java.util.Properties$LineReader.readLine(Properties.java:434)
    	at java.util.Properties.load0(Properties.java:353)
    	at java.util.Properties.load(Properties.java:341)
    	at JDBCUtil.JDBCutil.<clinit>(JDBCutil.java:20)
    	at JDBCUtil.JDBCTemplate.executeQueryMany(JDBCTemplate.java:86)
    	at Account_DAO.acount_Daoimpl.queryAllAccount(acount_Daoimpl.java:12)

问题分析

    1.properties文件置放位置不正确导致无法正确读取到指定文件，进一步造成了后续代码的空指针异常。

    2.properties文件位置正确后，发现复制过来的路径需要修改

java.sql.SQLSyntaxErrorException: ORA-00984: 列在此处不允许

问题描述

    SQL语句书写错误，没有正确输入

问题分析

    异常产生原因：当JVM从指定目录（ClassPath指定位置）中寻找需要的class文件时寻找失败

问题解决

    1.查看oracle.jdbc.OracleDriver 书写是否正确
    2.查看对应的jar包是否导入

2.SQLException

问题描述

    java.sql.SQLException: IO 错误: The Network Adapter could not establish the connection(JDBC无法跟oracle数据库网络适配器建立连接)

问题分析

    URL连接数据库需要的信息有误

问题解决

    查看url中给出的信息是否正确

3.UnsupportedClassVersionError

问题描述

    java.lang.UnsupportedClassVersionError:com/baizhi/demo/AccountMain : Unsupported major.minor version 51.0不支持的类版本异常，不支持版本51.0

问题分析

    JDK版本不一致

问题解决

    把项目所在的Eclipse改成项目原先的版本

4.

type Exception report

message Servlet execution threw an exception

description The server encountered an internal error that prevented it from fulfilling this request.

exception

    javax.servlet.ServletException: Servlet execution threw an exception
    	org.apache.tomcat.websocket.server.WsFilter.doFilter(WsFilter.java:52)

    由于构造方法中未包含所涉及的方法而抛出的异常

5.空指针异常NullPointerException

问题分析：

	在Action与View之间数值传递过程中，没有正确处理好数据，造成了数据丢失

问题解决：

重写
