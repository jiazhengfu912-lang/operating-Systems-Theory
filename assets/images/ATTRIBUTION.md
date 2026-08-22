# 外部图片署名与许可

本目录中的图片均以本地副本形式保存，避免依赖外部图片热链。每张图在使用章节旁也有中文导读、来源、许可和访问日期；本文件保留更完整的许可记录。

## `q004-ipc-kernel-bridge.svg`

- 标题：IPC：隔离进程如何通过操作系统协作
- 作者：本仓库为 Q004 绘制的原创 SVG
- 来源：无外部素材、无外部图片副本
- 许可：未单独声明许可；不得据此推定可独立转载、修改或再授权。
- 本仓库处理：原创文件，未使用第三方图像。

该图从“两个进程默认各有自己的虚拟地址空间”开始，比较两条常见 IPC 路径：共享内存由内核建立共同映射，消息传递由内核对象保存、排队或转交。它是教学简化图；没有表达所有 IPC 类型、缓存一致性、具体复制次数，或锁和信号量的完整实现。

## `q004-client-server-port.svg`

- 标题：客户端、服务器、端口与套接字
- 作者：本仓库为 Q004 绘制的原创 SVG
- 来源：无外部素材、无外部图片副本
- 许可：未单独声明许可；不得据此推定可独立转载、修改或再授权。
- 本仓库处理：原创文件，未使用第三方图像。

该图以一个 TCP Web 请求为例，展示客户端套接字、目标 IP、服务器监听端口、网络协议栈与服务器进程之间的关系，并特别提示端口不是进程也不是物理插孔。图中使用的是文档保留的示例 IP 地址；实际路由、NAT、IPv6、TLS 和多进程负载均衡等情况会更复杂。

## `q003-mmu-protection-path.svg`

- 标题：MMU 如何翻译地址并检查访问权限
- 作者：本仓库为 Q003 绘制的原创 SVG
- 来源：无外部素材、无外部图片副本
- 许可：未单独声明许可；不得据此推定可独立转载、修改或再授权。
- 本仓库处理：原创文件，未使用第三方图像。

该图用一个简化的“用户程序读取变量”场景，展示内核配置页表与权限、MMU 在硬件中逐次翻译与检查、允许访问 RAM 或当前无法直接完成而转交内核处理的完整路径。它不是任何具体 CPU 的电路图，也没有表达 TLB、缓存、多级页表或不同架构的全部细节。

## `q003-controlled-entry-events.svg`

- 标题：用户态程序进入内核的三条受控路径
- 作者：本仓库为 Q003 绘制的原创 SVG
- 来源：无外部素材、无外部图片副本
- 许可：未单独声明许可；不得据此推定可独立转载、修改或再授权。
- 本仓库处理：原创文件，未使用第三方图像。

该图对比普通应用最常遇到的系统调用、硬件中断和同步异常如何汇入 CPU 的受控入口，再让内核处理并受控返回。它采用常见教学模型；特定架构的入口名称、保存的现场以及返回指令会有所不同。

## `cpt-fetch-execute-mar-pc.svg`

- 标题：`CPT-fetch-execute-MAR-PC.svg`
- 作者：Pluke
- 原始页面：[Wikimedia Commons 文件页](https://commons.wikimedia.org/wiki/File:CPT-fetch-execute-MAR-PC.svg)
- 原始文件：[SVG](https://upload.wikimedia.org/wikipedia/commons/2/29/CPT-fetch-execute-MAR-PC.svg)
- 许可：CC0 1.0 Universal（公共领域贡献）
- 访问日期：2026-08-22
- 本仓库处理：原样保存，未修改。

该图用一个教学机的内存和寄存器，展示 `MAR ← [PC]` 这个取指步骤。它不是任何真实 CPU 的完整内部电路图。

## `virtual-address-space-physical-address-space.svg`

- 标题：`Virtual address space and physical address space relationship.svg`
- 作者：Stannered（描摹）；原作者 Dysprosia
- 原始页面：[Wikimedia Commons 文件页](https://commons.wikimedia.org/wiki/File:Virtual_address_space_and_physical_address_space_relationship.svg)
- 原始文件：[SVG](https://upload.wikimedia.org/wikipedia/commons/3/32/Virtual_address_space_and_physical_address_space_relationship.svg)
- 许可：3-Clause BSD License
- 访问日期：2026-08-22
- 本仓库处理：原样保存，未修改。

该图展示一个教学式、偏旧的 32 位地址布局。它只用于说明“虚拟地址连续、物理页框可离散、二者通过映射相连”的关系；不能据此推断现代系统的固定地址范围、区域排列或增长方向。

### 3-Clause BSD 许可声明

```text
Copyright © en:User:Dysprosia

Redistribution and use in source and binary forms, with or without modification,
are permitted provided that the following conditions are met:

1. Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.
2. Redistributions in binary form must reproduce the above copyright notice,
   this list of conditions and the following disclaimer in the documentation
   and/or other materials provided with the distribution.
3. Neither the name of en:User:Dysprosia nor the names of its contributors may
   be used to endorse or promote products derived from this software without
   specific prior written permission.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDER AND CONTRIBUTORS "AS IS" AND
ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```
