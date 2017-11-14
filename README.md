# tasker-common



## 说明
存放一些供其他tasker项目使用的公共模块
* 安装tasker
* 导入tasker项目

## 详细说明
* [comm_img_color.tsk] =>  
  获取指定图片的主色调  
  使用到模块[color-thief.min.js](https://github.com/lokesh/color-thief)修改部分代码
* [comm_wallpaper_color.tsk] =>  
  获取当前壁纸的主色调  
  调用模块[comm_img_color.tsk]

------------
* [comm_img_base64.tsk] =>  
  获取指定图片base64值  
  参数[图片路径;图片格式]，返回[图片base64值]
* [comm_base64_img.tsk] =>  
  使用base64值生成图片  
  参数[图片保存路径;图片格式][图片base64值]

------------

* [comm_color_rgb2hex.tsk] =>  
  将rgb颜色格式转为16进制格式[支持rgba格式]  
  参数[rgb颜色值]，返回[16进制颜色值]
* [comm_color_rgb2hex.tsk] =>  
  将透明度值[0-1]转为16进制格式  
  参数[透明度值]，返回[16进制透明度值]

------------
* [comm_img_path_vaild.tsk] =>  
  检验指定路径是否是正确的图片路径  
  参数[图片路径]，返回[是否正确]
* [comm_media_path2id.tsk] =>  
  获取media对应的id值，查询位置[content://media/external/images/media/]，主要用于查询图片  
  参数[图片源路径]，返回[图片id值]

------------
* [comm_img_width_height.tsk] =>  
  获取图片宽高值  
  参数[图片源路径]，返回[图片宽度;图片高度]
* [comm_img_crop_y.tsk] =>  
  对图片以高度为基准进行裁剪  
  参数[图片高度;图片宽度;图片源路径;图片保存路径]
* [comm_img_resize.tsk] =>  
  改变图片宽高，注意不会按照比例缩放  
  参数[图片宽度;图片高度;图片源路径;图片保存路径]
* [comm_img_scale.tsk] =>  
  对图进行裁剪，宽高不足按照比例裁剪  
  参数[图片宽度;图片高度;图片源路径;图片保存路径]
* [comm_img_draw_rect.tsk] =>  
  生成指定大小指定颜色的矩形图片  
  参数[矩形宽度;矩形高度;矩形颜色;图片保存路径]
* [comm_img_paint_png.tsk] =>  
  对指定图片进行油漆桶换色处理，会将所有非透明像素染成指定颜色  
  参数[颜色;图片源路径;图片保存路径]
  
------------
* [comm_img_blur.tsk] =>  
  对图片进行模糊处理  
  参数[源图片路径;图片保存路径;模糊程度;底部模糊区域百分比(可选)]  
  使用到第三方[stackblur.min.js](https://github.com/flozz/StackBlur)
* [comm_img_circle.tsk] =>  
  对图片进行圆形化处理  
  参数[主图缩放百分比;主图在副图x轴位置百分比;主图在副图y轴位置百分比;副图模糊程度]  
  使用到第三方[stackblur.min.js](https://github.com/flozz/StackBlur)
* [comm_img_HO.tsk] =>  
  对图片进行氢氧化处理  
  参数[图片宽度;图片高度;图片底部颜色;图片过渡部分样式(1-模糊 2-阴影);顶部实图高度百分比;图片源路径;图片保存路径]
* [comm_img_parallelogram.tsk] =>  
  对图片进行平行四边形化处理  
  参数[四边形高度百分比;四边形pos1位置Y值百分比;平行四边形角度值;副图模糊程度;图片源路径;图片保存路径]
* [comm_img_round_corner.tsk] =>  
  对图片进行圆角化处理  
  参数[圆弧半径;图片源路径;图片保存路径]

------------
* [comm_task_timer.tsk] =>  
  方便计算指定tasker任务运行时间