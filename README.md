### 项目名称
基于飞腾平台的Type-1型Hypervisor移植优化

### 描述
Type-1型Hypervisor在嵌入式领域以及ARM架构仍处于研究、开发和化阶段。因此，基于飞腾平台（ARMv8架构）的Type-1 Hypervisor的应用探索，有很大的创新空间，适合展示原创性

随着信创产业深化发展，国产处理器对虚拟化技术提出了更高要求，需要兼顾性能、安全和自主可控。飞腾CPU兼容ARMv8指令集，具备硬件级安全特性，为构建安全高效的虚拟化平台提供了良好基础。

本赛题将通过飞腾处理器平台与Type-1型Hypervisor的协同应用，探索在嵌入式系统中实现多内核、安全隔离及混合关键任务部署的可行路径，为构建新型智能终端系统提供实践基础。

### 导师
- 郭丁丁，guodingding1657@phytium.com.cn ，
- 刘晶晶，liujingjing1911@phytium.com.cn ，
- 郭霞，guoxia1873@phytium.com.cn ，

### 支持单位
飞腾信息技术有限公司

### 分类
虚拟化

### 难度
中

### 题目要求
参赛者需在飞腾CPU平台上实现虚拟化系统，可以从零做起，也可从基于开源Hypervisor移植优化。推荐开源方案（包括但不限于）：
- ZVM：Zephyr-based Virtual Machine，Type-1嵌入式RTOS虚拟化方案，基于Zephyr RTOS开发(C语言)
- Xvisor：轻量级Type-1 Hypervisor（C语言）
- Rust-Shyper：基于Rust语言内存安全型监控器
- AxVisor：基于ArceOS的模块化Hypervisor（Rust语言）
- seL4：Type-1微内核（C语言+ARM汇编）

参赛者需根据飞腾 CPU 的技术特点，选择合适的 Hypervisor 实现方案，完成虚拟化系统的开发与优化，并在飞腾平台上进行测试与验证，以满足高性能和安全性的要求。

### 预期目标
- 平台适配性：虚拟化系统需稳定运行于飞腾处理器平台
- 多虚拟机支持：同时运行至少两个相互隔离的虚拟机实例
- 生命周期管理：提供完整的虚拟机操作接口，包括：
- 虚拟机创建/销毁
- 运行状态控制（启动/暂停/恢复/终止）
- 资源监控（CPU/内存占用率）
- 跨VM通信：实现虚拟机间安全可控的通信机制（如共享内存+事件通知等）(可选)
- 性能优化：控制优化虚拟化开销(可选)
- 热迁移支持：实现虚拟机在同飞腾平台间的动态迁移(可选)

说明：上述目标供参考，参赛者可根据自身情况制定个性化方案或提出创新构想。

### 参考资料
- 飞腾派开发板资料
  - 百度网盘：https://pan.baidu.com/s/1pStiyqohrB3SxHAFFk8R6Q?pwd=dzdv  提取码：dzdv
  - iceasy商城飞腾派资料下载专区：https://www.iceasy.com/cloud/Phytium

- 飞腾开源项目资料
  - https://gitee.com/phytium_embedded
  - https://gitee.com/phytium_embedded/phytium-jailhouse
  - https://gitee.com/phytium_embedded/phytium-xen

- ZVMZephyr-based Virtual Machine
  - https://github.com/zephyrproject-rtos/zephyr/pull/84123
  - https://gitee.com/openeuler/zvm

- Rust-Shyper
  - https://gitee.com/openeuler/rust_shyper
  - https://www.openeuler.org/zh/blog/20230428-rust/20230428-rust.html

- Xvisor官方资料
  - https://xhypervisor.org/
  - https://github.com/xvisor/xvisor
  - https://github.com/xvisor/xvisor/blob/master/docs/arm/bcm2838-raspi4.txt

- sel4
  - https://github.com/seL4/seL4
  - https://github.com/au-ts/lionsos   
  - https://docs.sel4.systems/Tutorials/ 

- AxVisor
  - https://github.com/arceos-hypervisor/axvisor
 
### 备注
如需咨询赛题、申请开发板和加入赛题专项答疑群等其他相关事项，可添加赛事运营人员郭丁丁微信，添加好友时请注明“OS功能挑战赛+学校+姓名”。
![dfb88bfc-6789-4a9e-83b3-509c22d90eea](https://github.com/user-attachments/assets/fad5a542-8711-48d6-97c9-e37426a91e8e)

