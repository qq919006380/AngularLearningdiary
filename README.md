# 概念
- 组件：是angular应用的基本构建快，你可以把组件理解为一段带有业务逻辑和数据的HTML
- 模块：模块用来将应用中不同的部分组织成一个Angular框架可以理解的单元
- 路由：
---

# 命令
- ng new appName    ————生存新项目
    - ==注意：生成项目同时会下载npm依赖，如果失败需要换代理《nrm》==
- ng serve --open   ————启动服务器并监听文件变化， --open（或 -o）打开浏览器
---

- npm install -g @angular/cli ————安装最新版本
- npm install -g @angular/cli@1.5.2 ————安装指定版本 1.5.2
- npm uninstall -g @angular/cli ————卸载
- ng serve --port 4202 ————以4202端口打开服务
# angular-cli
- ng -v ————查看angular cli版本
- ng new xxx ————新建项目名称为XXX
- ng generate component xxx ————生成组件
- ng build  ————打包项目
    - ng build --prod   ————打包项目并且压缩
    - ==注意：在最新版本ng6+ 的cli加上--prod参数就自动AOT了==
- ng test   ————单元测试
# 类型描述文件
- 目的：让typescript认识jQuery和bootstrap，可以在ts文件中调用
- 安装本地
    - npm install @types/jquery --save-dev
    - npm install @types/bootstrap --save-dev
# 组件
- 值绑定[src]、事件绑定(click)、双向绑定[()]
- 内置结构指令
    - *ngIf、 *ngFor、 ngSwitch
- 内置属性指令
    - NGClass、NgStyle、NgModel
    - ==注意：NgModel只能用在表单上，一般结合双休绑定[(Ngmodel)]使用==
- 管道 过滤作用
    - public currentTime: Date = new Date();  //将currentTime过滤成指定格式
    - {{currentTime | date:'yyyy-MM-dd HH:mm:ss'}}
- 安全导航
    - {{currentRace?.name}} 如果currentRace没有name这个值则显示空，不会报错
---
- 组件通讯
    - 父子组件之间交互（@Input/@Output/模板变量/@ViewChild）
    - 非父子组件之间的交互（Service/localStorage）
    - 还可以利用Session、路由参数来进行通讯、请展开自己想象


    
