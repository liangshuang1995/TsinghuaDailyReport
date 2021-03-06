## 清华日报

学生健康和出行情况报告每日自动提交

强烈建议使用第二种方式，简单易行.


### 正常使用方式

* pip install -r requirements.txt
* 配置 conf.ini 输入清华info 用户名与密码
* python report.py
* 创建定时任务 Windows/Linux
> [Windows 创建定时任务](https://www.cnblogs.com/wensiyang0916/p/5773828.html)


### 非正常使用方式
> 如果你没有服务器，或者自己电脑也不能保证都开启，
那么Github Action可以作为你的服务器自动定时执行,并且非常安全。
>
* 创建github账户
* fork该仓库到你的项目，下面都是设置你的项目
* 进入: Settings-> Secrets-> 添加 USER_NAME 与 USER_PASS为你清华info的用户名与密码
![添加Secrets](https://github.com/naihaishy/TsinghuaDailyReport/blob/master/results/c.png)
* 进入: Actions 点击 Understand
![Understand](https://github.com/naihaishy/TsinghuaDailyReport/blob/master/results/d.png)

OK !

> 说明:Github Action的配置文件(.github/workflows/deploy.yml)中配置了时间 
默认是每天北京时间10:00 可以自行修改
>
> 不需要配置conf.ini 
>
> 运行日志去 Action下面查看
>
>高阶玩法可以配置邮箱, 参考: [GitHub Actions 教程：定时发送天气邮件](https://www.ruanyifeng.com/blog/2019/12/github_actions.html)

> Github Action服务器时间为UTC格式,比北京晚8个小时;
> 除此之外，它要慢几分钟(5分钟左右), 自己测试时多等待5分钟左右



### 效果图
![效果图1](https://github.com/naihaishy/TsinghuaDailyReport/blob/master/results/a.png) 
![效果图2](https://github.com/naihaishy/TsinghuaDailyReport/blob/master/results/b.png) 
![效果图3](https://github.com/naihaishy/TsinghuaDailyReport/blob/master/results/e.png) 
![效果图4](https://github.com/naihaishy/TsinghuaDailyReport/blob/master/results/f.png) 
