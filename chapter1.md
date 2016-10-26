## offset/scroll/client

* offsetWidth/offsetHeight:width/height + padding + border

* scrollWidth/scrollHeight:width/height + padding

*clientWidth/clientHeight:width/height + padding




## offset系列(./offset.png)
* 1.原生javascript中：
    + 1.1 offsetWidth和offsetHeight

    包括自身（宽）高度、内边距和边框，不包括外边距。

    + 1.2 offsetLeft和offsetTop

    从离自己最近的已经定位了的父亲元素开始算起。

    offsetLeft是以border的左上角开始计算；style.left是以margin的左上角开始计算

    也就是说，offsetLeft/offsetTop是包含外边距在内的

## scroll系列(./scroll.png)
* 1.原生javascript中：
    + 1.1 scrollWidth/scrollHeight

    实际内容的宽度和高度（即包括隐藏了的宽度和高度）
    + 1.2 scrollTop/scrollLeft

    已经卷起来的高度和宽度（包括边框在内）
    + 1.3 获取页面滚动坐标：
    var scrollTop = window.pageYOffset || document.documentElement.scrollTop || document.body.scrollTop || 0;

## client系列(./client.png)
* 1.原生javascript中：
    + clientWidth/clientHeight
    
    可是区域的宽高：内容宽高+padding，不包括

