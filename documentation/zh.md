<!-- ELUCENIA technical documentation · escore-air-apendicite · zh · no clinical/professional/rights approval -->

# AIR 评分（阑尾炎炎症反应）

[条件、来源与许可](https://elucenia.org/zh/tools/escore-air-apendicite)

## 使用方法

在门户中使用工具，或通过本地 HTTP 服务器打开 index.html。选择语言，填写各字段，然后计算。

## 输入与单位

### 呕吐

`vomito`

### 右髂窝疼痛

`dor`

### 反跳痛或肌卫

`defesa`

- `0` — 无
- `1` — 轻度
- `2` — 中度
- `3` — 重度

### 体温 ≥ 38.5 °C

`temp`

### 中性粒细胞

`neut`

- `0` — \< 70%
- `1` — 70 至 84%
- `2` — ≥ 85%

### 白细胞

`leuco`

- `0` — \< 10000/mm³
- `1` — 10.000 至 14.900 /mm³
- `2` — ≥ 15000/mm³

### C 反应蛋白

`pcr`

- `0` — \< 10 mg/L
- `1` — 10 至 49 mg/L
- `2` — ≥ 50 mg/L

## 方法版本

Andersson（2008）的AIR，采用2012年勘误更正后的表2和表7：七个组成项目，总分0–12，CRP单位为mg/L；原分组为0–4、5–8和9–12。未采用2021年提出的较低界值调整。

## 已记录的公式

呕吐（1）+ 右髂窝痛（1）+ 腹膜刺激轻（1）、中（2）、重（3）+ 体温≥38.5 °C（1）+ 中性粒细胞70–84%（1）或≥85%（2）+ 白细胞10000–14900（1）或≥15000（2）+ CRP 10–49（1）或≥50 mg/L（2）。总分0至12。

## 限制与适用人群

2008年的AIR研究纳入因疑似阑尾炎而入院的人群；部分受试者仍处于不确定组，需要进一步检查。2008年原文仅阅读了摘要。已直接阅读2012年的勘误：其中表2和表7更正了CRP浓度，并列明分值、单位和原分组。数值核对仅限于对七个已选项目求和；不认可临床分组，也不认可诊断、影像检查或手术决策。2021年的修订提出评分\<4为低风险，与原0–4组不同；本版本未采用这一调整。阅读2008年摘要并未确认最低年龄、排除标准或完整方案。未观察到的表现不得视为不存在。尚未进行独立专业人员的临床及语言审查，也未取得量表权利授权。

## 参考文献

- [Andersson M, Andersson RE. The appendicitis inflammatory response score: a tool for the diagnosis of acute appendicitis that outperforms the Alvarado score. World J Surg, 2008.](https://doi.org/10.1007/s00268-008-9649-y)

- [Di Saverio S et al. Diagnosis and treatment of acute appendicitis: 2020 update of the WSES Jerusalem guidelines. World J Emerg Surg, 2020.](https://doi.org/10.1186/s13017-020-00306-3)

- [Andersson M, Andersson RE. Erratum to: The Appendicitis Inflammatory Response Score: A Tool for the Diagnosis of Acute Appendicitis that Outperforms the Alvarado Score. World J Surg, 2012;36:2269–2270. Corrected Tables 2 and 7.](https://doi.org/10.1007/s00268-012-1679-9)

## 复现技术测试

在此仓库的根目录中运行 node test.cjs，以重复已记录的合成案例。原始输入、预期结果和容差保持不变。技术测试不构成临床验证。

```sh
node test.cjs
```

tool.json 包含来源、版本和审查范围。examples.json 保留合成输入与预期结果；results.json 记录实际得到的结果。

[记录与参考文献](../tool.json) · [JavaScript代码](../calculator.js) · [参考案例](../examples.json) · [results.json](../results.json)

## 审查与使用条件

尚未开展独立临床审查。

此界面为自主编写的翻译，并非官方或认证版本。尚未完成独立临床审查、专业语言审查或工具权利授权。

公式或分类结果。解释、处理及适用性须结合专业评估和所选来源。

## 许可与署名

Apache-2.0 仅适用于 ELUCENIA 代码。工具、出版物、翻译和数据的权利仍归各自权利人所有。请保留 LICENSE 和 NOTICE。

ELUCENIA · Felipe Guedes · Copyright © 2026
