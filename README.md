[toc]

# 2024.3.14
## 1. 学习vue框架，对接之前的项目
## 2. 尝试写前端页面，直接写新功能还未与后端接口联动
![](/imgs/1.png)
![](/imgs/2.png)
![](/imgs/3.png)

# 2024.3.27
## 1.继续学习vue框架，分别用临时数据和后端获取数据调试页面
![](/imgs/4.png)
## 2.优化界面显示和交互
![](/imgs/5.png)
## 3.vue和js学习经验
遇到了下图同样的问题
![](/imgs/6.png)
对象数组本质数组，有方法让vue响应，具体解决方式如下
1. 对于已经存在的数据，刷新vue列表元素渲染时的key值
![](/imgs/7.png)
2. 如果是新获取的数据，使用 $set 更新对象数组，此处对象内都是键值对形式的基本数据类型故可以用 ... 复制数据，如果有更复杂的数据类型应该要递归形成深拷贝
![](/imgs/8.png)

除此之外尝试同步写法试图获取更新数据后再让页面渲染或是让整个页面刷新都失败了，对vue和js各种实现的底层还不熟悉