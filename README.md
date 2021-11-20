# digitScroll

实现数字滚动的效果（领取红包后余额变化的数字滚动效果）

# 使用方法

- 包裹数字的容器设置高度，否则默认 30px
  例如

```
    <div class="wrapper">当前余额为<div id="digit-scroll"></div>元</div>
```

- 创建一个数字滚动实例，传入容器选择器

```
      const digitInstance = new DigitScroll({container:"#digit-scroll"});
```

- 在需要滚动的时候调用 roll 方法

```
        digitInstance.roll(78.48);
```

# 注意

装数字的容器是用 flex 布局的，如果要兼容比较低的浏览器版本的话，可以修改一下，把容器的 flex 布局去掉，每个数字的容器用 float:left 即可
即注释

```
      this.container.style.display = "flex";

```

然后解注释下面这一行

```
      // el.style.float='left';
```
      


