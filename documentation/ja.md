<!-- ELUCENIA technical documentation · escore-air-apendicite · ja · no clinical/professional/rights approval -->

# AIRスコア（虫垂炎の炎症反応）

[条件・出典・許諾](https://elucenia.org/ja/tools/escore-air-apendicite)

## 使い方

ポータルでツールを使用するか、ローカルHTTPサーバー経由でindex.htmlを開いてください。言語を選択し、項目を入力して計算してください。

## 入力項目と単位

### 嘔吐

`vomito`

### 右下腹部痛

`dor`

### 反跳痛または筋性防御

`defesa`

- `0` — なし
- `1` — 軽度
- `2` — 中等度
- `3` — 強い

### 体温 ≥ 38.5 °C

`temp`

### 好中球

`neut`

- `0` — \< 70%
- `1` — 70 ～ 84%
- `2` — ≥ 85%

### 白血球

`leuco`

- `0` — \< 10000/mm³
- `1` — 10.000 ～ 14.900 /mm³
- `2` — ≥ 15000/mm³

### C反応性蛋白

`pcr`

- `0` — \< 10 mg/L
- `1` — 10 ～ 49 mg/L
- `2` — ≥ 50 mg/L

## 方法の版

Andersson（2008）のAIRは、2012年の正誤表で訂正された表2と表7に基づく。七つの項目、合計0–12点、CRPの単位はmg/Lで、元の群分けは0–4、5–8、9–12である。2021年に提案された下限カットオフの変更は適用していない。

## 記載された計算式

嘔吐（1）+ 右下腹部痛（1）+ 腹膜刺激軽度（1）・中等度（2）・重度（3）+ 体温≥38.5 °C（1）+ 好中球70–84%（1）または≥85%（2）+ 白血球10000–14900（1）または≥15000（2）+ CRP10–49（1）または≥50 mg/L（2）。合計0～12。

## 限界・対象集団

2008年のAIRは、虫垂炎が疑われて入院した人を対象に研究され、対象集団の一部は判定保留群にとどまり、追加の検査を必要とした。2008年の原著は抄録のみを読んだ。2012年の正誤表は直接読み、その表2と表7ではCRP濃度が訂正され、配点、単位、元の群分けが示されている。数値の照合は、すでに選択された七つの項目の合計に限られ、臨床上の群分けや診断、画像検査、手術の判断を承認するものではない。2021年の改訂では、元の0–4群とは異なるスコア\<4の低リスク区分が提案されたが、この版では適用していない。2008年の抄録の読解では、最低年齢、除外基準、完全な手順は確認されていない。観察していない所見を存在しないものとして扱ってはならない。独立した専門家による臨床および言語の審査と、尺度の権利許諾は行われていない。

## 参考文献

- [Andersson M, Andersson RE. The appendicitis inflammatory response score: a tool for the diagnosis of acute appendicitis that outperforms the Alvarado score. World J Surg, 2008.](https://doi.org/10.1007/s00268-008-9649-y)

- [Di Saverio S et al. Diagnosis and treatment of acute appendicitis: 2020 update of the WSES Jerusalem guidelines. World J Emerg Surg, 2020.](https://doi.org/10.1186/s13017-020-00306-3)

- [Andersson M, Andersson RE. Erratum to: The Appendicitis Inflammatory Response Score: A Tool for the Diagnosis of Acute Appendicitis that Outperforms the Alvarado Score. World J Surg, 2012;36:2269–2270. Corrected Tables 2 and 7.](https://doi.org/10.1007/s00268-012-1679-9)

## 技術テストの再現

このリポジトリのルートディレクトリでnode test.cjsを実行すると、記録された合成ケースを再実行できます。元の入力、期待結果、許容誤差は保持されています。技術テストは臨床的検証を意味しません。

```sh
node test.cjs
```

tool.jsonには出典、版、確認範囲が記録されています。examples.jsonには合成入力と期待結果が保持され、results.jsonには実際に得られた結果が記録されています。

[記録・参考文献](../tool.json) · [JavaScriptコード](../calculator.js) · [参照ケース](../examples.json) · [results.json](../results.json)

## 確認状況と使用条件

独立した臨床レビューは実施されていません。

このインターフェースは独自に作成した翻訳であり、公式版や認証済みの版ではありません。独立した臨床レビュー、専門家による言語レビュー、評価尺度等の権利許諾の確認は実施されていません。

式または分類の結果です。解釈、対応、適用可能性は専門家による評価と選択した出典に依存します。

## ライセンスと帰属表示

Apache-2.0はELUCENIAのコードにのみ適用されます。評価尺度等、出版物、翻訳、データの権利は、それぞれの権利者に帰属します。LICENSEとNOTICEを保持してください。

ELUCENIA · Felipe Guedes · Copyright © 2026
