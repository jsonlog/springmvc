<!-- sed -i '' s/"t_news"/"T_NEWS"/g `grep -rl "t_news" --include=*.xml ./`
sed -i '' s/"t_sys_permission"/"T_SYS_PERMISSION"/g `grep -rl "t_sys_permission" --include=*.xml ./`
sed -i '' s/"t_sys_role"/"T_SYS_ROLE"/g `grep -rl "t_sys_role_permission" --include=*.xml ./`
sed -i '' s/"t_sys_role_permission"/"T_SYS_ROLE_PERMISSION"/g `grep -rl "t_sys_role_permission" --include=*.xml ./`
sed -i '' s/"t_sys_user"/"T_SYS_USER"/g `grep -rl "t_sys_user" --include=*.xml ./`
sed -i '' s/"t_sys_user_role"/"T_SYS_USER_ROLE"/g `grep -rl "t_sys_user_role" --include=*.xml ./`
sed -i '' s/"d_open_survey"/"D_OPEN_SURVEY"/g `grep -rl "d_open_survey" --include=*.xml ./`
sed -i '' s/"t_import_excel"/"T_IMPORT_EXCEL"/g `grep -rl "t_import_excel" --include=*.xml ./` -->
# springmvc 介绍 #

<pre>它是一个典型的MVC三层框架示例工程，快速简单的上手。</pre>

#### 涉及技术组件

+ SpringMVC
+ MyBaits
+ Apache Shiro
+ Bootstrap3
+ Sitemesh3
+ Activiti
+ log4j2；

### 集成示例
+ 用户登录
+ 文件上传下载
+ 文件压缩
+ Excel导入
+ JQuery联想搜索
+ Activiti工作流

### 效果
+ Activiti工作流
+ Shiro
+ SpringMVC MyBaits
+ log4j2
+ Bootstrap
+ Sitemesh3
+ 文件上传
+ 文件下载
+ JQuery联想搜索

#### 如何跑起来？
1. 初始化数据库以MySQL为例<br>
	a. 创建数据库demo<br>
	b. 创建activiti相关表，执行[ddl/activiti/mysql](ddl/activiti/mysql)目录下所有SQL脚本<br>
	c. 创建用户相关的基础表，执行[ddl/mysl/ddl.sql](ddl/mysql/ddl.sql)脚本<br>
	d. 导入测试数据，执行[ddl/mysl/init.sql](ddl/mysql/init.sql)脚本<br>
	e. 初始化一份测试用户数据，运行cn.springmvc.mybatis.init.InitServiceTest.[testInit()](src/test/java/cn/springmvc/mybatis/init/InitServiceTest.java)方法
	
2. 启动工程，访问: [http://ip:port/]( )


#### 用户体系授权？

> 用户组织权限相关表关系很简历，表之间的关联关系，可以看cn.springmvc.mybatis.init.InitServiceTest.[testInit()](src/test/java/cn/springmvc/mybatis/init/InitServiceTest.java)方法执行的步骤，这块就没有单独写页面来操作了


[GitHub](https://github.com/jsonlog) [issues](https://github.com/wangxinforme/springmvc/issues)

http://127.0.0.1:8080/springmvc/activiti/deployHome http://127.0.0.1:8080/springmvc/activiti/home http://127.0.0.1:8080/springmvc/activiti/listTask http://127.0.0.1:8080/springmvc/import/index http://127.0.0.1:8080/springmvc/news http://127.0.0.1:8080/springmvc/news/list http://127.0.0.1:8080/springmvc/upload/spring
http://127.0.0.1:8080/springmvc/user/register
http://127.0.0.1:8080/springmvc/upload/ajax