# tasker-common



## 说明
存放一些供其他tasker项目使用的公共模块
* 安装tasker
* 导入tasker项目
* [comm_wallpaper_color.tsk.xml] => 获取当前壁纸的主色调（使用到模块[color-thief.min.js](https://github.com/lokesh/color-thief)修改部分代码）（主用于配置scene背景色）
* [comm_image_base64.tsk.xml] => 获取指定图片base64值，参数[图片路径;图片格式]
* [comm_base64_image.tsk.xml] => 使用base64值生成图片，参数[图片保存路径;图片格式][图片base64值]
* [comm_rgb2hex_color.tsk.xml] => 将rgb颜色格式转为16进制格式[支持rgba格式]
* [comm_trans2hex_color.tsk.xml] => 将透明度值[0-1]转为16进制格式
* [comm_media_path2id.tsk.xml] => 获取指定media文件对应的media_id
* [comm_image_blur.tsk.xml] => 对指定图片进行模糊处理，参数[源图片路径;图片保存路径;模糊程度]（使用到模块[stackblur.min.js](https://github.com/flozz/StackBlur)）
* [comm_image_draw_rect.tsk.xml] => 生成指定大小矩形图片，参数[矩形宽度;矩形高度;矩形颜色;图片保存路径]
* [comm_image_paint_png.tsk.xml] => 对指定图片进行油漆桶换色处理，会将所有非透明像素染成指定颜色，参数[颜色;源图片路径;图片保存路径]