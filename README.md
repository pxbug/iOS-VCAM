VirtualCamera调整。将相机的图像/视频输出替换为任意的图像或视频文件。在iOS 15 - 17上测试

这通过连接到“mediaserverd”来工作，除其他外，mediaserverd负责连接到相机硬件并将图像数据转发给感兴趣的客户端（如用户安装的应用程序）。VCam在应用程序中工作，即使它们没有调整注入

这是POC阶段。“替换媒体”的文件路径在`image_utils.m`中硬编码。内存泄漏每30秒就会杀死“mediaserverd”

**图像文件**

---

<img src=".imgs/image.png" width="50%">

**视频文件**

---

<img src=".imgs/video.gif" width="50%">