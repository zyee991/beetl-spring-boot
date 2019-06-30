# beetl-spring-boot
## application.yml
```
spring:
  application:
    name: server-admin-web
  mvc:
    view:
      suffix: .html

beetl:
  templates-path: templates/
  config:
    #变量占位符的开始符号
    delimiter_placeholder_start:
    #变量占位符的开始符号
    delimiter_placeholder_end:
    #语句开始符号
    delimiter_statement_start:
    #语句结束符号
    delimiter_statement_end:
    #是否允许本地Class直接调用
    native_call: true
    ignore_client_io_error:
    #IO输出模式，默认是FALSE,即通常的字符输出，在考虑高性能情况下，可以设置成true
    direct_byte_output: false
    template_root:
    #模版字符集
    template_charset: UTF-8
    #异常解析类
    error_handler: org.beetl.core.ConsoleErrorHandler
    #是否进行严格MVC
    mvc_strict: false
    #扩展属性
    webapp_ext:
    #html标签支持（使用html类似标签调用标签函数或模版文件）
    html_tag_support: true
    #调用符号
    html_tag_flag: #
    import_package:
    #引擎实现类
    engine: org.beetl.core.engine.DefaultTemplateEngine
    # 本地Class调用的安全策略
    native_secuarty_manager: org.beetl.core.DefaultNativeSecurityManager
    #资源配置，resource后的属性只限于特定ResourceLoader
    resource_loader: org.beetl.core.resource.ClasspathResourceLoader
    #如果标签属性有var，则认为是需要绑定变量给模板的标签函数
    html_tag_binding_attribute: var
    function_tag_limiter:

```
