## Contents
- [第一次评审](#20240314)
- [第二次评审](#20240327)
- [第三次评审](#20240411)
- [第四次评审](#20240425)
- [第五次评审](#20240516)
- [第六次评审](#20240530)

## 2024.03.14
## 1. 学习vue框架，对接之前的项目
## 2. 尝试写前端页面，直接写新功能还未与后端接口联动
<!-- ![](/imgs/1.png) -->
<!-- ![](/imgs/2.png) -->
<!-- ![](/imgs/3.png) -->

## 2024.03.27
## 1.继续学习vue框架，分别用临时数据和后端获取数据调试页面
<!-- ![](/imgs/4.png) -->
## 2.优化界面显示和交互
<!-- ![](/imgs/5.png) -->
## 3.vue和js学习经验
遇到了下图同样的问题
<!-- ![](/imgs/6.png) -->
对象数组本质数组，有方法让vue响应，具体解决方式如下
1. 对于已经存在的数据，刷新vue列表元素渲染时的key值
<!-- ![](/imgs/7.png) -->
2. 如果是新获取的数据，使用 $set 更新对象数组，此处对象内都是键值对形式的基本数据类型故可以用 ... 复制数据，如果有更复杂的数据类型应该要递归形成深拷贝
<!-- ![](/imgs/8.png) -->

除此之外尝试同步写法试图获取更新数据后再让页面渲染或是让整个页面刷新都失败了，对vue和js各种实现的底层还不熟悉

## 2024.04.11
## 1. 将多次复用的页面顶部导航栏和底部元素抽离成组件，减少代码复用
在用户界面的各处都添加了这一组件，设计成第二次点击菜单按钮能返回主页的跳转方式，保留了首页独有的搜索框和进入收藏页后的图标（字符）变化
<!-- ![](/imgs/9.png) -->
<!-- ![](/imgs/10.png) -->
## 2. 分离界面时重新安排了文件内样式表的位置
css仍有较多的代码复用，还不明确是否可以统一成为全局样式表以及如何覆盖预先导入的样式
## 3. 写了用户保存多个地址的操作界面
只是一个架子，后续还要设计默认地址的显示方式
<!-- ![](/imgs/11.png) -->
<!-- ![](/imgs/12.png) -->

## 2024.04.25
## 1. 绘制架构图
<!-- ![](/imgs/15.png) -->
## 2. 完成网页app端地址相关内容
后端新增部分接口，完成需要的功能，提高效率
<!-- ![](/imgs/14.png) -->
在数据表存在自增主键并且后端接口没有返回索引信息的时候使用下图方式刷新全部数据
<!-- ![](/imgs/13.png) -->
## 3. 完成客户发起售后功能
尚不明确客户如何获得售后反馈
<!-- ![](/imgs/16.png) -->

## 2024.05.16
## 1. 完成支付宝支付后端
仅在沙箱环境中可用
沙箱买家账号 hggrrh0376@sandbox.com
沙箱买家登录密码 111111
沙箱买家支付密码 111111
<!-- ![](/imgs/17.png) -->
<!-- ![](/imgs/22.png) -->
## 2. 确定用户地址的使用逻辑
分析需求时仅设计用户可以预先设定地址字符串，收件人名与收件手机号需另外填写
可以选择地址也可以直接输入未录入的地址
<!-- ![](/imgs/20.png) -->
<!-- ![](/imgs/18.png) -->
<!-- ![](/imgs/19.png) -->
## 3. 初步实现支付宝支付前端
支付完成的跳转页面还没有确定/不知道如何跳转
<!-- ![](/imgs/21.png) -->
<!-- ![](/imgs/23.png) -->

## 2024.05.30
## 1. 安装银联支付SDK并调用
测试卡号：6216261000000000018
短信验证码（点击获取后才有效）：123456
![](/imgs/24.png)
![](/imgs/25.png)
## 2. 完善支付宝支付完成后的跳转
![](/imgs/26.png)
## 3. 梳理订单状态流程，画图
![](/imgs/27.png)
## 4. 前端增加不同支付方式的选项
![](/imgs/28.png)
![](/imgs/29.png)
## 5. 做完的功能做功能测试
[禅道](https://zjgsu.zentaopm.com/testcase-browse-261.html)