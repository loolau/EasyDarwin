# 项目来源 #
**EasyDarwin**项目来自[https://github.com/EasyDarwin/](https://github.com/EasyDarwin/)；

# EasyDarwin #

**EasyDarwin**是由国内开源流媒体团队维护和迭代的一整套开源流媒体视频平台框架，从2012年12月创建并发展至今，包含有单点服务的开源流媒体服务器，和扩展后的流媒体云平台架构的开源框架，开辟了诸多的优质开源项目，能更好地帮助广大流媒体开发者和创业型企业快速构建流媒体服务平台，更快、更简单地实现最新的移动互联网(安卓、iOS、H5、微信)流媒体直播与点播的需求，尤其是安防行业与互联网行业的衔接，EasyDarwin流媒体技术，助力传统行业升级转型！

## EasyDarwin开源项目（7Project） ##
EasyDarwin开源项目至今包括有：**EasyDarwin**（开源流媒体服务器）、**EasyCMS**（中心管理服务器）、**EasyCamera**（云摄像机服务）、**EasyClient**（云平台客户端）、**EasyAACEncoder**（开源音频编码项目）、**EasyAudioDecoder**（开源音频解码项目）、**EasyProtocol**（开源云平台协议）等多个项目，完整地构架了一套开源流媒体云平台方案：

1. **EasyCMS** 开源的设备接入与管理服务，支持多设备、多客户端接入，能非常快速地帮助大家实现稳定的设备接入服务，可以根据自己的需求进行服务功能拆分（例如用户接入服务与设备接入服务拆分等），具体见[https://github.com/EasyDarwin/EasyDarwin/tree/master/EasyCMS](https://github.com/EasyDarwin/EasyDarwin/tree/master/EasyCMS)；

1. **EasyDarwin** 核心流媒体服务！RTSP开源流媒体直播服务，高效、稳定、可靠、功能齐全，支持RTSP流媒体协议，支持安防行业需要的摄像机流媒体转发功能、支持互联网行业需要的多平台(PC、Android、IOS)**RTSP直播**（H264/MJPEG/MPEG4、AAC/PCMA/PCMU/G726）功能，底层(Select/Epoll网络模型、无锁队列调度)和上层(RESTful接口、WEB管理、多平台编译)、关键帧索引（秒开画面）、远程运维等方面优化，这些都是全代码完全开源的，具体接口调用方法和流程见：[https://github.com/EasyDarwin/EasyDarwin/tree/master/EasyDarwin](https://github.com/EasyDarwin/EasyDarwin/tree/master/EasyDarwin "EasyDarwin开源流媒体服务器")；

1. **EasyCamera** 设备端（摄像机、移动设备、桌面程序）对接EasyDarwin平台的方案，跨平台，支持Windows、Linux、ARM，其中EasyDarwin摄像机是我们定制的一款摄像机硬件与EasyDarwin平台进行对接的方案，摄像机采用海思3518E方案，支持RTSP、Onvif、WEB管理、配套SDK工具，作为开发和演示硬件工具，我们提供了全套完备的程序和文档，既可以用于流媒体学习，又可以用于方案移植参考，更可以直接用于项目中，用户可以将摄像机定制的部分替换成自己摄像机的硬件SDK，具体接入方法见[https://github.com/EasyDarwin/EasyCamera](https://github.com/EasyDarwin/EasyCamera)；

1. **EasyClient** 是EasyDarwin开源流媒体云平台的客户端实现，项目地址：[https://github.com/EasyDarwin/EasyClient](https://github.com/EasyDarwin/EasyClient "EasyClient")，功能包含：Windows、Android、iOS、H5(支持微信)四个部分，其主要功能包括：
	> - 云平台设备列表获取；
	> - 设备实时码流请求与播放；
	> - 设备云台控制；
	> - 设备语音对讲；

1. **EasyAACEncoder** 是一套简单、高效、稳定的开源音频编码库，支持将各种音频数据(G.711A/PCMA、G.711U/PCMU、G726、PCM)转码成AAC(with adts)格式，其中aac编码部分采用的是业界公认的faac库，EasyAACEncoder支持Windows、Linux、ARM等多种平台，能够广泛应用于各种移动终端设备、嵌入式设备和流媒体转码服务器！项目地址：[https://github.com/EasyDarwin/EasyAACEncoder](https://github.com/EasyDarwin/EasyAACEncoder "EasyAACEncoder")；

1. **EasyAudioDecoder** 是一套应用于移动端的简单、高效、稳定的开源音频解码库，能够将G.711A/PCMA、G.711U/PCMU、G726、AAC等音频格式转码到Linear PCM，再提供给流媒体播放器进行音频播放，EasyAudioDecoder支持跨平台，支持Android & iOS，目前已稳定应用于EasyPlayer、EasyClient等多个开源及商业项目！项目地址：[https://github.com/EasyDarwin/EasyAudioDecoder](https://github.com/EasyDarwin/EasyAudioDecoder "EasyAudioDecoder")；

1. **EasyProtocol** 是EasyDarwin开源流媒体服务器和开源平台使用的一套开源json协议，具有合理的结构设计、完善的层次逻辑以及简单精炼的调用接口，非常易于使用和扩展，不仅长期应用于EasyDarwin的服务器及平台中，而且能够快速扩展用户的自定义需求，非常好用！项目地址：[https://github.com/EasyDarwin/EasyProtocol](https://github.com/EasyDarwin/EasyProtocol "EasyProtocol")；

EasyDarwin RTSP流媒体服务器完全开源，EasyDarwin RTSP流媒体服务器在Darwin Streaming Server基础上做的优化和迭代，完全开源！后续也将继续扩展的录像、回放等多种服务和工具集，各个功能单元既可以独立使用于项目，又可以整体使用，形成一个完整、简单、易用、高效的流媒体解决方案！