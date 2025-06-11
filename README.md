# learning-log


## 2025/06/09
- Pythonのfor文を練習した
- GitHubで学習記録を始めた
- HTMLの< img >タグと< br >タグを使った

### メモ
- for _ in range(n): は、変数を使わないループ
- GitHubの「草」は活動ログを見える化してくれる！

### 明日以降の課題
- README.mdに画像リンクやコード例を追加して見やすくする  
- 毎日の記録を続けて、草を育てる  
- 就活でアピールできる見せ方をさらに工夫する  


## 2025/06/10
- マンション価格予測コンペ（Nishika）
- LightGBM を用いたモデル構築と評価
- カテゴリ変数（object型）を category 型に変換
- .cat.set_categories() を用いて train / test のカテゴリ整合性を確保
- ValueError: train and valid dataset categorical_feature do not match. の解消
- LightGBM のパラメータチューニング（early_stopping_rounds=50）
- カテゴリ変数の bin 数が多すぎる際の max_bin 警告に対処（警告のみ、無視可）
- submission.csv 作成・Nishika提出
- GitHubへの整理用コード構成案も確認
- 最終的に MAE: 0.0739998 を達成
- 暫定スコアは 0.1601

## メモ
- LightGBMではカテゴリ変数の一致が重要（set_categories()）
- astype('category') だけでは足りず、カテゴリのセット統一が必要
- 小さなエラーでも根本の理解が浅いと解決に時間がかかる
- cat アクセサが使えるのは category 型のみ（object型ではエラー）

## 次のアクション
- feature importance の可視化による改善点分析
- 他モデル（CatBoost, XGBoost）の比較検討
- GitHubにREADMEとノートブック整理してアップロード
