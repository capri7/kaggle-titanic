# kaggle-titanic

project_root/
│
├── README.md           # プロジェクトの概要と最終結論
├── data/               # データセットや前処理済みデータを格納
├── notebooks/          # 分析用のノートブック
├── models/             # モデル別の詳細を管理
│   ├── lightgbm/
│   │   ├── evaluation.md     # LightGBMの結果、評価指標、洞察
│   │   ├── implementation.md # LightGBMの実装手順やコードの詳細
│   │   ├── tuning.md         # ハイパーパラメータ調整の結果や洞察
│   │   └── ...
│   ├── catboost/
│   │   ├── evaluation.md
│   │   ├── implementation.md
│   │   └── ...
│   ├── xgboost/
│   │   └── ...
│   └── ...
├── results/            # 結果のグラフや重要なメトリクスを格納
└── scripts/            # 使用したスクリプトを保存

# Titanic Survival Prediction

This project focuses on predicting Titanic passenger survival using machine learning models. 
The most effective model was **LightGBM**, achieving an accuracy of 86.59% on the validation set.

## Key Results
| Model     | Accuracy | F1-Score | Notes          |
|-----------|----------|----------|----------------|
| LightGBM  | 86.59%   | 85.92%   | Best overall   |
| CatBoost  | 85.21%   | 84.45%   | Second-best    |
| XGBoost   | 84.78%   | 83.94%   |                |

For detailed insights, see:
- [LightGBM details](models/lightgbm/evaluation.md)
- [CatBoost details](models/catboost/evaluation.md)
