本插件基于英文版webpshop进行汉化。项目地址为：https://github.com/webmproject/WebPShop

基于Photoshop SDK 2021和WebP 1.2.1进行编译，请尽量使用2021版本PS。其他版本或许可用，但不保证其稳定性（原项目仅支持2021）

使用方法：将其放入PS安装目录下 Plug-ins 文件夹内，如果没有意外的话。可以在PS帮助菜单——>帮助——>增效工具下看到webp的版本信息。
本将会扩展PS的存储项，为其增加webp的保存选项。选择后，请参照下述文件描述，使用本插件功能。

编码设置 

质量滑块范围对应到 WebP 以下项：

|       质量滑块范围值     -> | 0    ...    97 | 98         99 |    100    |
|----------------------------|----------------|---------------|-----------|
|       WebP 编码设置     -> |    有损质量     |    近乎无损    |    无损    |
|                           |     0 ... 100   |   60 ... 80   |           |

单选按钮提供的压缩效果：

| 选项 |    WebP速度设置        |   YUV 锐化  |      WebP "质量" 设置     |
|      |                       |   (仅有损)  |           (非有损)        |
|------------------------------|-------------|--------------------------|
| 快速 |          1            |      No     |             0            |
| 默认 |          4            |      No     |            75            |
| 慢速 |          6            |      Yes    |           100            |

注意： 

  在 WebP 编码之前，16 和 32 位/通道被缩减为 8 位/通道，因为 WebP 内部仅支持 8 位。从 32 位文档导出应该在 WebP 编码设置中包含颜色配置文件，否则它们可能会比预期的更暗。
  WebP 图像不能超过 16383 x 16383 像素。
  不使用时间线数据；因此动画依赖图层来定义帧（在每个图层的名称中将持续时间设置为“（123 ms）”），并且在保存之前需要对其进行栅格化处理。
  在某些图像上，无损压缩可能会产生比有损压缩更小的文件大小。这是因为质量滑块不是线性的原因。控制压缩效果的单选按钮也存在同样的问题。
  无论相关的复选框状态如何，颜色配置文件始终应用在 Windows 上的预览图像，而不会应用于macOS。
  此插件不会扩展 导出——>存储为Web所用格式。
  编码和解码将依次完成。目前无法中断取消该操作，大图像可能需要一些时间。
  仅支持最新的 Photoshop（2021）版本。
