# CQ-picfinder-robot-add-on

给Tsuk1ko大佬的CQ-picfinder-robot V2.4做了几个自用小挂件，非常不完善  
大部分功能是稳定的，有一些bug不知道什么时候可以填上  
   **注意！！！** main已魔改，2.4以外的版本不一定可以直接用


## 部件列表  

### 1. 涩图分类  
可以请求不同种类的涩图，数据库为本地储存的MongoDB，setu_database里是我自己扒了10多个tag并手工删减了一些不太行的，可以用MongoDB恢复到数据库，不需要的话可以自己用pxer扒  
点餐语句为 给我康康xx

### 2. 自动获取新微博  
定时检查指定账号是否有发新微博，如果有就自动发出来，包含文字图片和视频，  
从微博移动版获取的内容，无需登录但是需要找你想看的人的uid，countainerID = 107603+uid（也不知道为什么加107603就管用）  
可以用特定语句开启或者关闭自动检查功能，语句为“自动检查新微博”，偶尔会抽风  
也可以手动要求看哪一条微博，比如 “看看**方舟上条**微博”，方舟和上条可以改，可以要求看置顶，上条，上上条，上上上条.....

### 3. 看漫画  
实现了自动翻页，暂停自动翻页，跳页，手动翻页之类的功能  
可以和狗群员一起看漫画，没什么卵用，语句是 看看漫画  
需要指定本地漫画的地址（对你得把漫画下载到本地），从1.jpg开始

### 4. 获取少前新人/皮肤的大破图  
来源是少前台服官网，需要手动触发，语句为“康康新枪/皮肤”

### 5. 骰子  
可以扔出任意面数（<1000），任意个数(<10)的骰子，可以指定最小值，自动统计总分  
用法的话，举个栗子，.d20x3,5 表示3个最低为5的d20  
（偷懒直接写main里面了）

### 6. 少前帮助  
问问题可以给出对应的NGA的网址链接  
（偷懒直接写main里面了）

### 7. 少前战区分数统计(能用，有bug，几率报错)  
也用了MongoDB...可以输入分数然后查看分数（写了一半！）
@机器人然后用以下格式  
战区 游戏名称:xxxx；分数：xxxxxx；排行：xx  
（不用打百分号，注意用分号隔开每项内容）
