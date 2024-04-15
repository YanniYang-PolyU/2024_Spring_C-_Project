# 2024_C++_Project（2024春季c++课程 大作业）
This is the project for the 2024 spring C++ course.

## Project Description (大作业描述)
本次大作业要求：为山东大学青岛校区食堂写一个反馈系统——饕在山青——*山东大学青岛校区餐厅反馈系统*。

### Admin & User（关于系统管理员和用户两种用户）
该系统的用户分为两种：管理员（admin）和学生/老师用户（user），他们有不同的属性和操作。
- 管理员
    - 属性：账号（8位数字），密码（9位数字）
    - 操作：登录、添加新管理员、删除已有管理员、修改管理员密码、添加菜色、删除菜色、查看用户反馈
    - 注：
        - 关于管理员登录、添加和删除管理员：admin.txt文件中预先存放了系统初始时的默认管理员信息，登录操作通过查看admin.txt文件中是否存在相应账号，并验证密码是否一致；添加和删除管理员需相应向admin.txt中添加/删除管理员账号及其密码信息。
        - 关于添加和删除菜色：dishes.txt文件用于存放菜色信息，关于菜色的相关信息，请查看后续菜色相关的要求。

- 学生/老师用户
    - 属性：姓名（拼音形式，如张三一，Sanyi Zhang）, 账号（学号或职员号），密码（数字或字母，位数自定）
    - 操作：用户登录、查看所有菜色、搜索菜色、提交意见。
    - 注：
        - 关于用户登录：users.txt文件中预先存放了在校生和老师的名字、学号/职员号、初始密码（身份证后六位），登录操作通过查看users.txt文件中是否存在相应名字和账号，并验证密码是否一致。
        - 关于查看所有菜色、搜索菜色：查看所有菜色是将dishes.txt文件中的菜色信息显示出来；搜索菜色是给定菜色名，显示该菜色的详细信息。
        - 提交意见：输入意见，并将其保存到comments.txt文件中。

### Dish (关于菜色)
菜色的重心在其各种属性上，当然也会有相应的关于菜色的操作。
- 属性：菜名、食材、地点（餐厅、楼层、窗口）、价格
- 操作：请根据【管理员中的添加/删除菜色】操作所需，自行定义。
- 注：菜色有很多种，比如炒菜类、粉面类、清真类等等，我们这里要求对不同菜色种类进行不同处理
    - 至少要有炒菜类、粉面类两种菜色，在以上菜色基础属性的基础上，根据不同类型的菜色添加新的属性/操作；比如，粉面类的数据会有口味（清汤、酸辣、麻辣...）和加料（牛肉、肠、煎蛋...）等新的属性。

### Requirement（要求）
- 实现以上功能，在命令行中模拟系统的运行，模拟运行过程可以参考提供的“EatAtSDUQ.exe”（我自己手搓代码得到的可执行文件，仅供参考，不合理之处同学们可以自行修改）。
    - 完成管理员相应的功能：得到30%的分数
    - 完成用户相应的功能：得到25%的分数
    - 满足菜色的相应要求：得到25%的分数
    - 顺利模拟系统的运行：得到10%的分数
    - 指出目前系统设定的不足，添加一项你觉得需要的新功能，解释添加新功能的原因和实现逻辑：得到10%的分数
    - Bonus: 将命令行系统用界面（QT或者其他框架）来实现，可以得到额外10%的分数。
- 需提交：
    - 报告1份（PDF格式，写清楚你设计系统的逻辑和系统的组件，可以辅以UML图、流程图等）
    - 代码（包括源文件、头文件等）
    - 自己代码编译、连接生成的可执行文件（一定要确保自己的可执行文件可以直接运行，助教会通过该exe文件来测试你的功能）
    - 将以上文件打包成一个压缩文件，并以“姓名+学号+大作业”命名，发送到相应的助教处（平时实验发送的助教，记得设置邮件回执）。
    - 大作提交截止日期：5月26日晚10点！
    - 大作提交截止日期：5月26日晚10点！
    - 大作提交截止日期：5月26日晚10点！
