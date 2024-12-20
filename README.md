# TMS320F28335 SCIB 实现程序

## 资源描述

本仓库提供了一个基于 TI 的 TMS320F28335 DSP 芯片的 SCIB（串行通信接口 B）实现程序。该程序使用 CCS6.0 开发环境编写，适用于研旭实用开发板。程序实现了 DSP 与串口调试助手之间的通信，提供了两种实现方式：查询方式和 FIFO 中断方式。

## 功能特点

1. **查询方式**：
   - 实现字符和字符串的接收与发送。
   - 通过查询 SCIB 的状态寄存器来判断数据是否准备好。

2. **FIFO 中断方式**：
   - 实现可变数据长度的字符串数据发送与接收。
   - 使用 FIFO 中断来处理数据，提高数据传输效率。

## 文件结构

- `source_code/`：包含用 CCS6.0 编写的源码文件。
- `serial_debug_tool/`：包含一个串口调试助手，使用非常方便。

## 使用说明

1. **开发环境**：
   - 使用 CCS6.0 开发环境进行编译和调试。
   - 确保开发板与计算机通过串口连接。

2. **编译与下载**：
   - 打开 CCS6.0，导入源码文件。
   - 编译项目并下载到 TMS320F28335 开发板上。

3. **串口调试**：
   - 使用提供的串口调试助手进行通信测试。
   - 根据需要选择查询方式或 FIFO 中断方式进行数据传输。

## 注意事项

- 确保开发板与计算机的串口连接正确。
- 在使用 FIFO 中断方式时，注意中断处理函数的编写，避免数据丢失。

## 贡献

欢迎提交问题和改进建议，帮助我们完善这个项目。

## 许可证

本项目采用 MIT 许可证，详情请参阅 `LICENSE` 文件。

## 下载链接

[TMS320F28335SCIB实现程序](https://pan.quark.cn/s/e56740cc4381)