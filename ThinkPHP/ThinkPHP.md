# ThinkPHP

>
>
>

## 基础介绍

### think
```yaml
think:
    make:controller: 资源控制器
    make:middleware: 中间件
    make:validator: 验证器
    run: 运行
```

### 目录结构
```yaml
目录结构:
    /app:
        /controller:
            Index.php:
        /middleware:
        /model:
        /validate:
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
        /cache:
        /log:
        /session:
        /storage:
    /vendor:
    /view: 视图模板
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
        $middleware:
        validate():
    Request:
        $filter:
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
        Cache:
        Cookie:
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
        Filesystem:
        Request:
        Route:
            allowCrossDomain():
            delete():
            domain():
            ext():
            get():
            group():
            https():
            middleware():
            miss():
            only():
            option():
            pattern():
            prefix():
            resource():
            rest():
            rule():
            token():
            vars():
        Session:
        View:
            engine():
            fetch():
    file:
        UploadedFile:
    middleware:
        SessionInit:
    model:
        concern:
            SoftDelete:
        Pivot: 中间表
    paginator:
        driver:
            Bootstrap:
                render():
                total():
    App:
        getBasePath():
    Cache:
        clear():
        delete():
        get():
        inc():
        pull():
        push():
        set():
        tag():
    Collection:
        toArray():
    Cookie:
        get():
        set():
    Filesystem:
        putFile():
    Image:
        crop():
        open():
        rotate():
        save():
        thumb():
        water():
        width():
    Model: 模型
        $disuse:
        $name:
        $pk:
        $readonly:
        $schema:
        allowField():
        attach():
        belongsToMany():
        count():
        create():
        delete():
        destory():
        detach():
        find():
        force():
        getData():
        getFieldAttr():
        has():
        hasMany():
        hasOne():
        hasWhere():
        init():
        limit():
        onEvent():
        onlyTrashed():
        order():
        paginate():
        replace():
        save():
        saveAll():
        searchFieldAttr():
        select():
        setFieldAttr():
        together():
        update():
        visible():
        where():
        with(): 预加载
        withAttr():
        withCount():
        withSearch():
        withTrashed():
    Request:
        action():
        buildToken():
        checkToken():
        file():
        has():
        host():
        isPost():
        method():
        only():
        param():
        post():
        session():
        url():
    Response:
        code():
    Session:
        all():
        clear():
        delete():
        get():
        has():
        pull():
        set():
    Validate:
        $message:
        $rule:
            email:
            file:
            max:
            require:
        $scene:
        batch():
        check():
        getError():
        isNumber():
        rule():
        scene():
    captcha_check():
    cookie():
    env():
    input():
    json():
    redirect():
    request():
    response():
    session():
    url():
    view():
```



### 路由





### 控制器




#### 请求



#### 响应




### 中间件



### 视图


### 验证器



### 数据库



#### 模型


模型事件：
- onAfterRead:
- onBeforeInsert():


