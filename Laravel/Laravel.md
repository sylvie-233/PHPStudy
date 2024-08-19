# Laravel

>
>`#TODO 30 Days to Learn Laravel P6`
>

## 基础介绍

### laravel & artisan
```yaml
laravel:
    new:

artisan:
    db:seed: 数据库填充
    key:generate: 生成APP_KEY
    migrate: 数据库迁移
    serve: 开启服务
```

### 目录结构
```yaml
laravel:
    /app:
        /Http:
            /Controllers:
        /Models:
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
        /factories:
        /migraions:
        /seeders:
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
    Broadcasting:
    Bus:
    Cache:
    Config:
    Console:
    Container:
    Contracts:
    Cookie:
    Database:
        Eloquent:
            Factories:
                HasFactory:
                    create():
                    factory():
        Migrations:
            Migration:
        Schema:
            Blueprint:
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
    Log:
    Mail:
    Notifications:
    Pagination:
    Pipeline:
    Process:
    Queue:
    Redis:
    Routing:
    Session:
        SessionServiceProvider:
    Support:
        Facades:
            Artisan:
            Blade:
                component(): 注册组件
            Hash:
            Route:
                get():
            Schema:
                create():
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
    env():
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
    @class: css类属性
    @csrf:
    @each: 循环导入其它页面
    @empty:
    @env:
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


### Error Handling


### Logging