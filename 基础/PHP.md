# PHP
>
>`#TODO [完结]猫叔2024php8零基础从入门到精通快速入门教程 P12`
>

## 基础介绍



### php
```yaml
php:
    -r:
    -v: 版本
```




## 核心内容
```yaml
Affecting PHP's Behaviour:
    Error Handling and Logging:
        trigger_error(): 生成错误信息
Command Line Specific Extensions:
    Readline:
        readline(): 输入一行
File System Related Extensions:
    Filesystem:
        copy(): 复制文件
        dirname(): 获取目录
        fgets(): 从文件中读取一行
        file_exists(): 文件存在判断
        unlink(): 删除文件
Other Basic Extensions:
    SPL:
        spl_autoload_register(): 自定义autoload
Text Processing:
    Strings:
        echo(): 输出字符串
        print(): 输出字符串
        strtr(): 字符串替换

Variable and Type Related Extensions:
    Array:
        array(): 创建数组
    Class/Object Information:
        is_subclass_of():
    Function Handling:
        call_user_func():
    Variable handling:
        gettype(): 获取变量类型
        var_dump(): 输出变量信息
```

### 预定义
```yaml
预定义变量:
    $argc:
    $argv:
    $_COOKIE:
    $_ENV:
    $_FILES:
    $_GET:
    $_POST:
    $_REQUEST:
    $_SERVER:
    $_SESSION:
    $GLOBALS:
```




### 数据类型
```yaml
Types:
    array:
    Booleans:
    Floating:
    Integers:
    Mixed:
    Never:
    null:
    Objects:
    Resources:
    string:
    Void:
```


#### 字符串
```php
$str = "xxxx"

// 字符串拼接
$str = "aaa" . "bbb"


/// 多行字符串
$str = <<<EOF
    字符串内容
EOF;
```
双引号字符串支持模板字符串








#### 数组
```php
$arr = ["1", "2", "3"]
```






### 控制流程






### 面向对象




### 命名空间


### 属性



### PDO






