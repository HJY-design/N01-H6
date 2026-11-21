# N01 H6 硬件工程

两种文件均从同一份立创发布工程导出。嘉立创 EDA 专业版使用 `easyeda/N01-H6.epro`。Altium Designer 使用 `altium/N01-H6-Altium.zip`，解压后按原目录结构打开 `Board1_1.PrjPcb`。ZIP 内含工程、七页 `.SchDoc` 和一份 `.PcbDoc`。PCB ASCII 单文件约 114 MiB，所以用 ZIP 保留完整 AD 项目和相对路径。

两种格式均核对到 256 个 PCB 元件、201 个名称一致的 PCB 网络和 815 条过孔记录。AD 工程的 8 个文档引用齐全。焊盘相关记录由两种格式分别表达，数量不能直接用来比对焊盘几何。检查封装、铺铜、阻焊和规则时请同时对照原生工程。格式转换说明见[嘉立创导出指南](https://prodocs.lceda.cn/cn/import-export/export-altium-designer/)。

N01 自研原理图和 PCB 采用 [CERN-OHL-W-2.0](../LICENSE)。
