# Laravel

>
>`#TODO 30 Days to Learn Laravel P21`
>

## 基础介绍

### laravel & artisan
```yaml
laravel:
    new:

artisan:
    db:seed: 数据库填充
    help: 帮助命令
    key:generate: 生成APP_KEY
    make:controller: 生成控制器
    make:factory: 生成工厂模型
    make:mail:
    make:migration: 生成数据库迁移
    make:model: 生成模型
        -m: 生成迁移文件
    make:policy:
    migrate: 数据库迁移
    migrate:fresh:
        --seed:
    migrate:refresh: 重置迁移
    queue:work:
    route:list:
    serve: 开启服务
    tinker: shell交互
    vender:publish:
```

### 目录结构
```yaml
laravel:
    /app:
        /Http:
            /Controllers:
        /Mail:
        /Models:
        /Policies: Gate封装
        /Providers:
    /bootstrap:
        /cache:
        app.php:
        providers.php:
    /config:
        app.php:
        auth.php:
        cache.php:
        database.php:
        filesystems.php:
        logging.php:
        mail.php:
        queue.php:
        services.php:
        session.php:
    /database:
        /factories: 使用模型工厂生成假数据（到数据库）
        /migraions: 数据库迁移
        /seeders: 数据库填充(使用factory填充)
    /public:
    /resources:
        /css:
        /js:
        /views: Blade页面
    /routes:
        web.php: web路由配置
    /storage:
        /app:
        /framework:
            /cache:
            /sessions:
            /testing:
            /views:
        /logs:
    /tests:
        /Feature:
        /Unit:
    /vendor:
    .env:
        APP_KEY:
    artisan:
    phpunit.xml:
    vite.config.js:
```



## 核心内容
```yaml
Illuminate:
    Auth:
        Access:
            Gate:
    Broadcasting:
    Bus:
        Queueable:
    Cache:
    Config:
    Console:
    Container:
    Contracts:
        Auth:
            attempt(): 尝试登录
            guest():
            login(): 登录
            logout():
            user():
        Queue:
            ShouldQueue:
    Cookie:
    Database:
        Eloquent: ORM框架
            Collection:
            Factories:
                HasFactory:
                    create(): 生成假数据
                    factory():
            Model: ORM模型
                $fillable:
                $table:
                all():
                attach():
                belongsTo(): 属于关联
                belongsToMany():  多对多关联
                create():
                delete():
                find():
                hasMany(): 拥有管理
                hasOne():
                links(): 分页链接
                paginate():
                preventLazyLoading(): 禁用懒加载
                save():
                update():
                with(): 预加载关联模型
        Migrations:
            Migration:
        Schema:
            Blueprint:
                foreignIdFor(): 外键定义
                id():
                nullable():
                string():
                unique():
        Seeder:
    Encryption:
    Events:
    Filesystem:
    Foundation:
        Auth:
            User:
        Configuration:
            ApplicationBuilder:
                create():
                withExceptions():
                withMiddleware():
                withRouting():
                    web:
                    commands:
                    health:
            Exceptions:
            Middleware:
        Console:
            ClosureCommand:
        Application:
            configure:
        Inspiring:
    Hashing:
    Http:
        Request:
            is(): url匹配
            validate(): 字段校验
    Log:
    Mail:
        Mailables:
            Content:
                view:
            Envelope:
        Mailable:
    Notifications:
    Pagination:
        Paginator:
            defaultView():
            userBootstrap():
    Pipeline:
    Process:
    Queue:
        SerializesModels:
    Redis:
    Routing:
    Session:
        SessionServiceProvider:
    Support:
        Facades:
            Artisan:
            Blade:
                component(): 注册组件
            Gate: 验证拦截
                authorize():
                define():
            Hash:
            Mail:
                queue():
                send():
                to():
            Route:
                controller():
                get():
                group():
                middleware():
                post():
                resource(): 
                view():
            Schema:
                create():
            Vite:
                asset():
        Arr: 数组工具类
            first():
        ServiceProvider:
            boot():
            register():
        Str:
    Testing:
    Translation:
    Validation:
        ValidationServiceProvider:
    View:
        Component: 自定义组件
            render():
        View:
    dispatch():
    env():
    fake():
    logger():
    request():
    view():
```





### Routing


### Middleware



### Controllers



### Views



### Blade Templates


#### Displaying Data

`{{ $xxx }}`：显示数据

属性绑定：可直接在prop前加上符号`:`，和Vue一样


#### Blade Directives
```yaml
Blade指令:
    @auth:
    @can: 权限校验
    @cannot:
    @class: css类属性
    @csrf:
    @each: 循环导入其它页面
    @empty:
    @env:
    @error: 错误校验判断
    @extends: 继承模板
    @for: 列表渲染
    @foreach:
    @forelse:
    @guest:
    @hasSection:
    @if:
    @include: 导入其他页面
    @includeIf:
    @isset:
    @method: 指定表单方法
    @once:
    @php: php代码
    @production:
    @props: 定义组件可传递属性
    @session: 段落填充
    @sectionMissing:
    @style: css样式属性
    @switch:
    @unless:
    @use: 导入php类
    @vite:
    @while:
    @yield:
```

#### Components

匿名组件：`<x-componentName>`位于`resources/views/components`目录，会自动进行注册

组件内容通过php变量`$slot`传递、组件css属性通过php变量`$attributes`传递，其它属性可直接传递

自定义插槽传递：`<x-slot:slotName>`、在组件中使用`$slotName`显示内容


#### Layout





### ORM



### Validation

字段校验错误会在页面传递`$errors`变量


### Error Handling


### Logging