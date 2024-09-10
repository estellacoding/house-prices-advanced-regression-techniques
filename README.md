# 房價預測

## 概述
房價預測專案目的是預測每棟房屋的銷售價格

## 使用模型
1. **FLAML(Fast and Lightweight AutoML)**
    - 訓練過程中，FLAML探索多個模型(如LightGBM、XGBoosting、Random Forest、CatBoost等)
    - 最終，CatBoost模型在眾多候選模型中表現最佳，達到了最低的RMSE(0.1250)
    - 模型選擇的過程花費了大約14948.7秒(約4小時9分鐘)

## 評估標準
本次比賽用於評估的衡量標準是均方根誤差。
$RMSE = \sqrt{\frac{1}{n} \sum_{i=1}^{n} (y_i - \hat{y}_i)^2}$

## 提交分數
最後使用最佳模型(CatBoost)提交至Kaggle，提交分數為 **0.12752**