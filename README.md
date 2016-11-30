# QPHelperKit
最近一直利用闲时准备着QPHelperKit开源项目，目标是降低项目开发成本。目前已发布v0.1.0版本，已经具备最基本的功能，可极大的减少开发成本，提高开发效率。后续会继续维护，也将会在公司的项目中使用，一直迭代着！

# QPPhotoBrower

```
// 允许用户交互
_imageView.userInteractionEnabled = YES;

// 引入QPPhotoBrower类之后,为自己需要放大的imageView添加tap手势
UITapGestureRecognizer *tapGesture = [[UITapGestureRecognizer alloc]initWithTarget:self action:@selector(magnifyImage)];
[_imageView addGestureRecognizer:tapGesture];
```

```
- (void)magnifyImage
{
    NSLog(@"局部放大");
    [QPPhotoBrower showImage:self.imageView]; // 调用方法
}
```
