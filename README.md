# JLInputView
实现微信输入框效果（textView自适应文字高度），用法如下：
```objc
    // 1.设置文本框占位文字内容以及字体颜色
    _inputView.placeholder = @"请输入内容";
    _inputView.placeholderColor = [UIColor lightGrayColor];
    
    // 2. 监听文本框文字高度改变
    _inputView.textHeightChangeBlock = ^(NSString *text,CGFloat textHeight){
    
          
   
    };
    
    //3.设置文本框最大行数
    _inputView.maxNumberOfLines = 4;
```
效果图：

![效果图](https://github.com/JlongTian/JLInputView/blob/master/image/show.gif)
