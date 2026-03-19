# 接口性能测试项目（JMeter分布式）
## 项目说明
基于JMeter搭建Master-Slave分布式压测环境，对JSONPlaceholder接口做阶梯加压测试，找到性能拐点。
## 测试环境
- 压测机：阿里云ECS（2核2G）
- JMeter版本：5.6.3
- 被测接口：https://jsonplaceholder.typicode.com/
## 测试流程
50→100→200→300→400并发，每级跑60秒，监控TPS/响应时间/CPU使用率。
## 目录说明
- jmx/：JMeter脚本
- raw-data/：压测原始数据
- reports/：HTML报告
- charts/：性能趋势图
- docs/：测试文档