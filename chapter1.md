## offset/scroll/client

* offsetWidth/offsetHeight: width/height + padding + border
* scrollWidth/scrollHeight: width/height + padding
* clientWidth/clientHeight: width/height + padding



## offset系列 ![Alt text](./offset.png)
* 1.原生javascript中：
    + offsetLeft和offsetTop

    从离自己最近的已经定位了的父亲元素开始算起。

    offsetLeft是以border的左上角开始计算；style.left是以margin的左上角开始计算

    也就是说，offsetLeft/offsetTop是包含外边距在内的

## scroll系列![Alt text](./scroll.png)
* 1.原生javascript中：
    + scrollTop/scrollLeft

    已经卷起来的高度和宽度（包括边框在内）
    + 获取页面滚动坐标：
    var scrollTop = window.pageYOffset || document.documentElement.scrollTop || document.body.scrollTop || 0;

## client系列![Alt text](./client.png)
    + 网页可视区宽高
    var clientWidth = window.innerWidth || document.documentElement.clientWidth || document.body.clientWidth || 0;

