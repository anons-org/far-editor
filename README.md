# far-editor

#### 介绍
##### 为什么要开发farEditor
- 研究、学习集成开发环境下，语言服务器，调试协议的实现。
- 满足小众游戏开发圈子中缺少代码编辑器的刚性需求
- 最后，通过该项目，参与人员能对市面上软件领域，芯片领域、操作系统领域、高级语言虚拟机的代码编辑器、调试器的实现做到心中有数。


#### 设计碎语
布局可以参考vscode
- [ ] 创建项目（创建一个新的文件夹就是一个项目，项目的配置文件就在该文件内）
- [ ] 打开项目（根据目录地址打开一个项目）
- [ ] 树形展开项目的代码文件，支持折叠和展开
- [ ] 右边为table区域，可以展示文件的代码以及代码行。（第一个版本不需要代码提示，关键字高亮、语法检查） 代码行 支持添加、删除、禁用断点
#### 1.0 核心功能
- 设置断点
- 删除断点
- 禁用断点
- 断点触发时：
> 根据语言服务器返回的协议，讲指定的代码行标红
> 在A区域显示当前所有的线程（下拉列表）
> 在B区域展示当前栈帧中的所有局部变量(树形控件）可以直接添加ROOT（此动作为：添加需要监视的变量）
> 在C区域显示单行执行，进入，跳出 等按钮

- 核心功能中 线程、局部变量 都由语言服务器推送，前端负责显示即可 

#### v1.1功能
- 代码文件列表，支持修改文件名，删除文件， 添加文件



