# 🎵 XiaoMusic Web Theme for IPhone

> 基于 **XiaoMusic** 的一个纯前端 Web 主题  
> 专为 **iPhone / iOS Safari** 适配优化，接近独立app的使用感  
> 单文件 `index.html` 即可部署

---

## 📱 项目简介

这是一个为 XiaoMusic 打造的移动端 Web 播放主题，重点解决：

- ✅ iPhone Safari 播放适配
    
- ✅ 锁屏播放控制
    
- ✅ 灵动岛显示
    
- ✅ 耳机线控支持（上一曲 / 下一曲 / 暂停）
    
- ✅ 媒体中心控制
    
- ✅ 封面 & 歌词自动刮削展示

- ✅ 支持MusicFree插件

- ✅ 支持自定义歌单
    

完全单 HTML 文件，无依赖构建工具。

---

## 📦 部署方式

### 🔧 安装方式  
只需将文件 **`iwebplayer.html`** 复制到 XiaoMusic 的 `static` 目录下：
- Docker 方式（示例命令）：
```bash
docker cp /home/路径/iwebplayer.html 容器名称:/app/xiaomusic/static/iwebplayer/iwebplayer.html
```
### ▶️ 使用方式
- 在iPhone Safari浏览器访问 http://XiaoMusic地址:端口/static/iwebplayer/iwebplayer.html
  
💡 建议将该 URL 共享到手机桌面，这样更像独立的APP。


---

## 📷 效果示意


<!-- 第1行 -->
<p>
  <img src="https://github.com/user-attachments/assets/b9069276-33e6-4ea1-9b74-cb7fe5ae0675" alt="效果图1" width="300">
  &nbsp;&nbsp;&nbsp;&nbsp;
  <img src="https://github.com/user-attachments/assets/9bf69bf1-4902-4045-a0fe-eb01e6c0af90" alt="效果图2" width="300">
  
</p>

<!-- 第2行 -->
<p>
  <img src="https://github.com/user-attachments/assets/3491706d-1101-4f1b-bae9-e0906e2a1c26" alt="效果图3" width="300">
  &nbsp;&nbsp;&nbsp;&nbsp;
  <img src="https://github.com/user-attachments/assets/06208e9f-c983-4f5d-be13-4db7e8a76c77" alt="效果图4" width="300">
</p>

<!-- 第3行 -->
<p>
<img src="https://github.com/user-attachments/assets/58dfbdf3-e532-4716-8b73-df92a53f1b62" alt="效果图5" width="300">
 &nbsp;&nbsp;&nbsp;&nbsp;
<img src="https://github.com/user-attachments/assets/82c85ddb-fba1-4227-ba52-ae331f5b5bd1" alt="效果图5" width="300">

</p>    

<!-- 第4行 -->
<p>
<img src="https://github.com/user-attachments/assets/004063df-c94a-482d-80e9-ededf444c31a" alt="效果图5" width="300">
 &nbsp;&nbsp;&nbsp;&nbsp;
<img src="https://github.com/user-attachments/assets/0ea9ee6b-771a-49c4-8b46-a37ee51796a6" alt="效果图5" width="300">
  
</p>    

---



## ✨ 核心特性

### 🎶 播放功能

- 本机播放
    
- 远程设备播放（多设备切换）
    
- 单曲循环 / 列表循环 / 随机播放
    
- 音量控制（本机 + 远程设备）
    
- 设备在线状态监测
    
- 远程播放轮询同步
    

---

### 🖼 封面 + 歌词刮削

- 自动获取封面
    
- 自动解析 LRC 歌词
    
- 高亮滚动歌词
    
- 封面旋转动画
    
- 无歌词自动降级展示


    

---
    

## 🧠 技术实现

### 使用技术

- 原生 HTML
    
- 原生 CSS（无框架）
    
- 原生 JavaScript
    
- MediaSession API
    
- iOS 适配优化
    
- CSS 动态主题变量
    
- SVG 图标内嵌
    

无：

- ❌ Vue
    
- ❌ React
    
- ❌ jQuery
    
- ❌ 打包工具
    
- ❌ 第三方播放器库
    

---

## 🔌 后端接口依赖

该主题基于 XiaoMusic 提供的接口运行：

/musiclist  
/musicinfo  
/getsetting  
/device_list  
/playingmusic  
/setvolume  
/getvolume  
/cmd  
/proxy/music

支持新版 `/proxy/music`，自动探测兼容旧版 `/proxy`。

---

## 🧩 工作模式

### 本机模式

- 浏览器直接播放
    
- 支持进度拖动
    
- 支持本地音量控制
    
- 支持锁屏控制
    

---

### 远程设备模式

- 控制 XiaoMusic 设备播放
    
- 实时同步播放状态
    
- 同步播放模式
    
- 同步音量
    
- 离线设备自动灰显
    

---


## 🎛 播放模式说明

|模式|说明|
|---|---|
|单曲循环|当前歌曲循环|
|列表循环|顺序播放|
|随机播放|随机切歌|

本机模式使用 LocalStorage 保存状态  
远程模式读取设备播放模式 



---

## 🚀 项目目标

- 打造一个 iPhone 完整可用的 XiaoMusic Web 播放主题
    
- 提供接近原生 App 的体验
    
- 保持部署极简
    
- 保持后端零侵入
    

---

## 📜 License

仅作为 XiaoMusic 的 Web 主题扩展使用。  
请遵循 XiaoMusic 本体项目的相关协议。

---

## ❤️ 致谢

iWebPlayer 基于 XiaoMusic 官方项目开发：
👉 https://github.com/hanxi/xiaomusic

感谢原作者 hanxi 提供优秀的后端服务接口。
iWebPlayer 仅作为其生态下的一个 Web 主题扩展。
