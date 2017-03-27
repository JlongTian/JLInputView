# JLInputView
实现微信输入框效果（textView自适应文字高度）头文件如下
```objc
#import <UIKit/UIKit.h>

@interface JLInputView : UITextView
/**
 *  textView最大行数
 */
@property (nonatomic, assign) NSUInteger maxNumberOfLines;

/**
 *  文字高度改变block → 文字高度改变会自动调用
 *  block参数(text) → 文字内容
 *  block参数(textHeight) → 文字高度
 */
@property (nonatomic, strong) void(^textHeightChangeBlock)(NSString *text,CGFloat textHeight);

/**
 *  设置圆角
 */
@property (nonatomic, assign) NSUInteger cornerRadius;

/**
 *  占位文字
 */
@property (nonatomic, strong) NSString *placeholder;

/**
 *  占位文字颜色
 */
@property (nonatomic, strong) UIColor *placeholderColor;
/**
 *  是否需要隐藏占位文字
 */
@property (nonatomic,assign) BOOL placeholderHidden;

@end
```
