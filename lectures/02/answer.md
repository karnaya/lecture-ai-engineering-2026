# 第2回 解答

## 演習

- 使ったモデル・設定（`result.json` の `config` から）：Qwen/Qwen3.5-0.8B（revision 2fc0636）、LoRA（量子化なし）、lora_r=16、lora_alpha=32、lr=2e-4、num_train_epochs=20、seed=42、貪欲生成（do_sample=False）
- 自分で学習を実行したか（`executed_training_myself`）：はい
- 学習前：`format_rate` = 0.095（2/21） / `content_rate` = 0.0（0/21）
- 学習後：`format_rate` = 1.0（21/21） / `content_rate` = 0.905（19/21）
- 退行した質問：無し
- 学習後に残った失敗と、その型（根拠なしの質問に断定した / 根拠ありの質問に確認要求で逃げた / 形式の崩れ）：根拠なしの質問に断定した
- 知識を問う質問（セクション 6）の結果（学習前の分類 → 学習後の分類）と気づいたこと：
  - 最終課題の締切（FAQ に無い）：format_error → asserted（FAQ の提出期限をそのまま流用）
  - 担当教員の名前（FAQ に無い）：format_error → needs_review
  - 次回の講義のテーマ（FAQ に無い）：format_error → needs_review
  - 課題の提出期限（対照・FAQ にある）：format_error → asserted（正答）
  - 気づいたこと：採点時に○とされていても回答としては不自然なものが存在する。
- 学習で変わったこと・変わらなかったこと：形式は揃うが、似た内容がFAQにあるとそれに引っ張られる。

## 宿題

- 取り組んだレベル：基礎 / 実装 / 発展
- 変えた設定やデータ：
- 結果（比較表や数字）：
- ファインチューニングが向く場面・向かない場面についての考察：
