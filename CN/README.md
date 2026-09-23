# 中文指南

这是一个以双端短读长 RNA-seq 为例的实践记录，覆盖从原始 FASTQ 到表达计数与功能注释的基本流程。

## 章节

1. [质量控制](1.quality_control.txt)：使用 fastp 清洗双端 reads 并生成 QC 报告
2. [比对](2.alignment.txt)：准备参考基因组/注释，使用 HISAT2 比对，并用 samtools 排序和建立索引
3. [定量与注释](3.quantitive.txt)：使用 StringTie 生成计数矩阵，并使用 gffread、TransDecoder、eggNOG-mapper 进行后续注释

英文版见 [English guide](../EN/README.md)。

## 使用前请确认

- 本仓库是学习笔记和命令模板，不是可直接用于生产环境的自动化流程。
- 示例针对 paired-end 数据；文件命名约定为 `<sample>_1.fq.gz` 和 `<sample>_2.fq.gz`。
- 运行前请替换所有示例路径、样本名、线程数以及参考文件名。
- 参考 FASTA 与 GTF/GFF 必须来自同一组装版本，且染色体/contig 名称需要一致。
- 建议记录每个软件的版本、命令和日志，并先用少量样本测试。
