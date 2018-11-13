# 项目命名规范

## Package

包命名规则是为了防止不同组织开发的 Java 代码发生命名冲突。给包起名字，要把组织的 Internet 域名每个部分倒转，比如组织的域名是 `domain.com`，包名称使用 `com.domain` 前缀，然后再加上项目、模块和代码包名称。比如 `com.domain.project.module.service`。

有时候域名里的字符不能作为合法的包名称，要遵循以下规则：

- 如果域名含有中划线，用下划线代替，比如：`com.info_world`；
- 如果域名含有保留字，在后面加一个下划线，比如：`com.int_`；
- 如果域名以数字开头，或者其他不合法的字符，在前面加一个下划线，比如：`net._5460`.

包名称的第一部分可以使用全小写的顶级域名，包括`com`, `edu`, `gov`, `mil`, `net`, `org`，也可以遵循 ISO 3166 标准采用两位字符国家代码，参考：[ISO 3166 Codes (Countries)](https://baike.baidu.com/item/ISO%203166-1). 中国的代码是 `cn`.

域名定义更明细的包名称，一般采用单位分支、部门、项目名称、功能模块等名称，例如：

- com.domain.hr.service
- edu.somecompany.department.socket
- com.cucs.productname.v2

为了避免与类和接口名称发生冲突，包名称全部使用小写字符。

