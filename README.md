# BREATH₂ Score Calculator (Web, static)

軽量・クライアントサイドのみで動く **BREATH₂スコア** 計算ツール（Saito Y, et al., 2025 準拠）。
スマホ/PCのブラウザで動作し、サーバ通信は行いません（PHI/個人情報は保存しません）。

## デモ（GitHub Pages）
このリポジトリを GitHub Pages（`main` ブランチ / `root`）で公開すれば、
`https://<your-account>.github.io/<repo-name>/` で誰でも利用できます。

## 使い方
1. 年齢、BNP/NT-proBNP、Hb、CTR、CAD、AF、ECG-LVH を入力/チェック
2. 自動で 0–9 点を算出し、低/中/高リスクを表示
3. 「印刷/保存」でPDF化、「結果をコピー」でJSON出力

## スコア配点（Saito Y, et al., 2025）
- BNP/NT-proBNP 高値：**2点**
- 年齢 ≥ 65：**2点**
- 心房細動：**1点**
- CTR ≥ 50%：**1点**
- 冠動脈疾患既往：**1点**
- 貧血（男 < 13 / 女 < 12 g/dL）：**1点**
- ECG-LVH（Sokolow-Lyon: RV5 + SV1 ≥ 3.5 mV）：**1点**

## 安全・プライバシー
- すべて **ブラウザ内で完結**（外部送信なし）
- 患者氏名やIDなどの **個人情報入力欄はありません**
- 医療判断の補助であり、**診断を確定するものではありません**

## ライセンス
MIT License. 詳細は `LICENSE` を参照してください。

---
*References:*
- Saito Y, et al., 2025. BREATH₂ score for HFpEF screening.
- Public summaries by Gunma Univ. and medical media.
