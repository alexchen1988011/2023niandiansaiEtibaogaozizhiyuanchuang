# 2023年电赛E题资源报告(自制原创)

## 资源描述

本资源严格按照官方对报告的内容和格式要求编写，为原创自制，请勿盗卖或转载。该资源详细介绍了“运动目标控制与自动追踪系统”的设计与实现。该系统以MSP432P401R为控制核心，结合OpenMV视觉系统，实现了对摄像头中出现的红色激光、绿色激光、屏幕边线、黑色胶带等目标的识别与处理。

## 系统架构

该系统采用两块MSP432P401R控制核心，分别控制两台二维电控云台。第一台云台上安装红色激光笔，主控根据接收到的屏幕边线的坐标信息控制电控云台带动红色激光在屏幕边线上进行移动。第二台云台上安装绿色激光笔，主控根据接收到的红色激光的坐标位置控制电控云台带动绿色激光进行追踪。

## 关键技术

1. **视觉识别**：使用OpenMV摄像头对红色激光、绿色激光、屏幕边线、黑色胶带进行识别，并将处理结果发送给MSP432P401R控制核心。
2. **增量式PID算法**：采用增量式PID算法对坐标信息进行处理，减少目标位置与实际位置的误差，从而实现对云台的精确控制。
3. **双控制核心**：系统采用两块MSP432P401R控制核心，分别控制两台电控云台，实现运动目标的控制与自动追踪功能。

## 系统功能

1. **红色激光控制**：根据屏幕边线的坐标信息，控制红色激光在屏幕边线上移动。
2. **绿色激光追踪**：根据红色激光的坐标位置，控制绿色激光进行自动追踪。
3. **误差校正**：通过增量式PID算法，减少目标位置与实际位置的误差，提高系统的稳定性和精度。

## 注意事项

- 请勿盗卖或转载本文，尊重原创作者的权益。
- 系统设计与实现过程中严格按照官方要求进行，保证报告的完整性和准确性。

## 适用对象

本资源适用于参加2023年电赛E题的参赛者，以及对运动目标控制与自动追踪系统感兴趣的电子爱好者和研究人员。

## 下载链接
[2023年电赛E题报告自制原创](https://pan.quark.cn/s/c45a5467e262) 

(备用: [备用下载](https://pan.baidu.com/s/1AQo7fY4ycM4wMZvodLJEeQ?pwd=1234))
