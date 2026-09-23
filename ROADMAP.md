# Roadmap / 待补充内容

The current repository is a useful hands-on record, but the following additions would make it reproducible and safer to reuse.  
当前仓库已经记录了主要步骤；以下内容会让流程更可复现、更适合复用。

## High priority / 高优先级

- [ ] Add a sample-sheet template with sample ID, read paths, condition, replicate, and strandedness.
- [ ] Add an environment lock file or container with tested tool versions.
- [ ] Add a small public test dataset and expected checksums/results.
- [ ] Add automated input checks for missing read pairs, duplicate sample IDs, and FASTA/GTF contig mismatches.
- [ ] Add MultiQC aggregation for fastp, HISAT2, and samtools reports.
- [ ] Document library strandedness and pass the correct setting to downstream quantification.
- [ ] Document biological replicates, normalization, experimental design, and differential-expression analysis.

- [ ] 增加样本表模板：样本 ID、read 路径、分组、重复与链特异性。
- [ ] 增加经过测试的软件版本锁定文件或容器。
- [ ] 增加小型公开测试数据、校验值和预期结果。
- [ ] 自动检查 read 配对缺失、样本 ID 重复以及 FASTA/GTF contig 不一致。
- [ ] 使用 MultiQC 汇总 fastp、HISAT2 和 samtools 报告。
- [ ] 说明文库链特异性，并在定量步骤中正确设置。
- [ ] 补充生物学重复、归一化、实验设计和差异表达分析。

## Medium priority / 中优先级

- [ ] Convert the Chinese chapters from plain text to Markdown and align section names with the English guide.
- [ ] Replace machine-specific paths with a configuration file.
- [ ] Add a workflow engine (Snakemake or Nextflow) with resumable steps.
- [ ] Add checksums and provenance for reference FASTA/GTF files.
- [ ] Add annotation-validation guidance instead of ad hoc line deletion.
- [ ] Add resource estimates for memory, threads, disk space, and scheduler examples.
- [ ] Add citations for fastp, HISAT2, samtools, StringTie, gffread, TransDecoder, GeneMark, and eggNOG-mapper.

## Nice to have / 可选

- [ ] Add CI checks for shell syntax, Markdown links, and example configuration.
- [ ] Add `CONTRIBUTING.md`, issue templates, and a citation file.
- [ ] Add separate paths for reference-guided quantification and novel-transcript discovery.
- [ ] Compare gene-level counting options such as featureCounts with the StringTie workflow.
