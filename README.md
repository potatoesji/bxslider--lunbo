#[bxslider--lunbo官方网站](https://bxslider.com/options/ "https://bxslider.com/options/")--------[git地址](https://github.com/stevenwanderski/bxslider-4 "https://github.com/stevenwanderski/bxslider-4")

##bxslider插件---双向控制轮播图

bxslider插件 
   左右按钮切换  --点击左右按钮时 没有限制 造成连续点击时 会一下滚动好几张图片的现象

   `解决方案：等上一次运动完成后再执行左右按钮的点击`

   `实施方法：el.isWorking()  
        在el.goToNextSlide()和 el.goToPrevSlide() 中 判断是否在工作状态  
        el.isWorking()值true的话 就不向下执行      
        el.isWorking()false 就执行下一步`

##添加功能 scroll
    `scroll值为true时  允许鼠标滚轮控制轮播 ; false时 则不允许
    具体添加方法--- 模拟keyboardEnabled依次添加相关内容`
