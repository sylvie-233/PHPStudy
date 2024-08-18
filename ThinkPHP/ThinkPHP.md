# ThinkPHP

>
>`#TODO 【李炎恢】ThinkPHP8.x | 后端框架课程 | 已完结 | 共50p P31`
>

## 基础介绍

### think
```yaml
think:
    run: 运行
```

### 目录结构
```yaml
目录结构:
    /app:
        /controller:
            Index.php:
        /model:
        .htaccess:
        AppService.php:
        BaseController.php:
        common.php:
        event.php:
        ExceptionHandle.php:
        middleware.php:
        provider.php:
        Request.php:
        service.php:
    /config:
        app.php:
        cache.php:
        console.php:
        cookie.php:
        database.php:
        filesystem.php:
        lang.php:
        log.php:
        middleware.php:
        route.php:
        session.php:
        trace.php:
        view.php:
    /extend:
    /public:
        index.php: 对外入口文件
        router.php:
        .htaccess:
    /route:
    /runtime:
    /vendor:
    /view:
    .example.env:
    .travis.yml:
    composer.json:
    think:
```

#### 配置信息
```yaml
database.php:
    connections:
        mysql:
            type:
            hostname:
            database:
            username:
    default:
route.php:

```




## 核心内容
```yaml
app:
    BaseController:

think:
    db:
        Query:
            chunk():
            column():
            count():
            cursor():
            dec():
            delete():
            exp(): 表达式
            field():
            find():
            inc():
            insert():
            insertAll():
            insertGetId():
            limit():
            max():
            min():
            replace():
            save():
            select():
            strick():
            update():
            value():
            where():
            whereExp():
            whereLike():
            whereOr():
            whereRaw():
            withAttr():
    facade:
        Db:
            execute():
            getLastSql():
            name():
            query():
            raw(): 原始sql
            rollback():
            startTrans():
            table():
            transaction():
            
    model:
        concern:
            SoftDelete:
    App:
        getBasePath():
    Collection:
        toArray():
    Model: 模型
        $disuse:
        $name:
        $pk:
        $readonly:
        $schema:
        allowField():
        belongsToMany():
        count():
        create():
        delete():
        destory():
        find():
        force():
        getData():
        getFieldAttr():
        hasMany():
        hasOne():
        hasWhere():
        init():
        limit():
        onEvent():
        onlyTrashed():
        order():
        replace():
        save():
        saveAll():
        searchFieldAttr():
        select():
        setFieldAttr():
        update():
        where():
        withAttr():
        withSearch():
        withTrashed():
    Request:
        action():
    env():
    json():
```



### 路由





### 控制器




#### 请求



#### 响应


#### 中间件



### 视图


### 验证器



### 数据库



#### 模型


模型事件：
- onAfterRead:
- onBeforeInsert():


