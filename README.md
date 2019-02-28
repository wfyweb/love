# nav-dome

这是一个导航，主要功能用键盘跳转相对应的网站；

1.html

创建kbd标签（定义键盘文本。）
点击出现自定义输入框

2.html

动态创建kbd标签：

利用JSON对象获取数据while循环创建kbd

点击后输入网站

 事件委托 e['targer']     e['terget']['id']
 
 记录点击元素，输入的信息
 
 设置本地缓存 localStorage.setItem('zzz', JSON.stringify(hash))


3.html
 // 取出 localStorage 中的 zzz 对应的 hash
 
 localStorage.setItem( "name",ogj )
 localStorage.getItem( "name" )

4.html
封装函数，方便调用。

  1. 初始化数据
    var hashA = init()
    var keys = hashA['keys']
    var hash = hashA['hash']

   2. 生成键盘
    遍历 keys，生成 kbd 标签
    generateKeyboard(keys, hash)

   3. 监听用户动作
    listenToUser(hash)



##  更新
1. 键盘样式
2. icon位置
3. img 加载错误处理
4. 相关代码分块， 封装为函数
