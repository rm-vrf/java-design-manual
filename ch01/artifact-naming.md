# 构件产物命名规范

构建产物命名由 `groupId`, `artifactId`, `version` 三个部分组成，其中 `artifactId` 和 `version` 中间加一个下划线，后面加扩展名，构成了产物文件名。比如：`jettison-1.3.7.jar`

- `groupId` 是构建产物的唯一标识，需要区别其他组织的项目和构件产物。遵循 Java 包命名规范，`groupId` 的第一部分是倒置的域名，然后加上单位分支、部门、项目名称、功能模块等名称。

  比如：`com.mydomain.hr.myproject`

  `groupId` 可以继续细分，与项目结构保持一致。如果是一个多模块项目，可以在 `groupId` 后面加上模块名称。

  比如：`com.mydomain.hr.myproject.reporting`, `com.mydomain.hr.myproject.plugins`

- `artifactId` 是 jar 文件的名称，使用小写字母、数字和中划线组成，不要含有文件名中不允许出现的特殊字符。

- `version` 由数字和点组成，比如：1.0, 1.1, 1.0.1, 不要使用日期，除非是 SNAPSHOT 构建。



