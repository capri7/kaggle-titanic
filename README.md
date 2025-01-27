### "Titanic"

Body:
The Titanic is widely known as a luxury ocean liner; however, when analyzing the passenger class distribution and ticket fares, a different narrative emerges.

Key Observations:
Passenger Distribution: Pclass 3 passengers accounted for more than half (55.1%) of the total, suggesting a reliance on lower-class passengers for revenue. On its maiden voyage, only 1,317 passengers boarded, just 53% of the ship’s capacity, while the crew count remained at 907.

Fare Analysis: The average fare for Pclass 1 was more than six times higher than Pclass 3, highlighting a stark economic divide between passenger classes.

Lifeboat Shortage: While outdated maritime safety regulations are the primary reason for insufficient lifeboats, financial constraints might have played a role. For example, prioritizing cargo over additional lifeboats could have been seen as a cost-saving measure.

These observations suggest that the Titanic operated under significant financial and operational pressures, balancing luxury, revenue, and safety—an imbalance that tragically contributed to the disaster.

# タイタニックデータセット分析から得られる主要な洞察

タイタニック号は豪華客船として広く知られていますが、乗客階級の分布やチケット料金を分析すると、異なる視点が浮かび上がります。タイタニック号はその豪華さで有名ですが、実際には多くの移民労働者を輸送する船としての役割も果たしていた可能性があります。

## 主な観察点

### 乗客分布
Pclass 3（3等客室）の乗客は全体の55.1%を占めており、収益面で3等客室の乗客に大きく依存していたことが示唆されます。処女航海では、乗客数はわずか1,317人で、船の定員の53%に過ぎませんでした。一方で、乗務員の数は予定通り907人が確保されていました。

### 料金分析
Pclass 1（1等客室）の平均運賃はPclass 3の6倍以上であり、乗客階級間での経済的格差が浮き彫りになっています。また、Kaggleの`train`データセットに基づくと、乗客1人当たりの平均運賃は約**32.20**でした。

### 救命ボート不足
救命ボートの不足は、時代遅れの海上安全規則が主な原因であると広く考えられていますが、財務的な制約も影響を与えた可能性があります。たとえば、追加の救命ボートよりも貨物スペースを優先することが収益性の観点から合理的であると見なされたのかもしれません。

---

## 結論

これらの観察結果は、タイタニック号が豪華さ、収益、安全性の間で大きな財務的および運営上のプレッシャーを受けていたことを示唆しています。このようなバランスの欠如が、経済的には正当化される一方で、災害時には悲劇的な結果を招く意思決定につながった可能性があります。






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
| Model            | Accuracy | 
|------------------|----------|
| Random Forest    | 79.42%   | 
| Ensembele        | 78.23%   | 
| Gradient Boost   | 78.73%   | 
| LightGBM         | 77.99%   | 
| SVC              | 77.51%   | 
| Stacking         | 77.51%   | 
| CatBoost         | 77.27%   | 
| XGBoost          | 76.79%   | 

For detailed insights, see:
- [LightGBM details](models/lightgbm/evaluation.md)
- [CatBoost details](models/catboost/evaluation.md)
