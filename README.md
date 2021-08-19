# kaggle-Optiver Realized Volatility Prediction
## 2021/08/17
- [Optiver Realized Volatility Prediction](https://www.kaggle.com/c/optiver-realized-volatility-prediction)に参加


## 2021/08/18
- データ理解, 可視化を実施<br>
参考記事: 
  - [Optiver Realized : EDA for starter(日本語version)](https://www.kaggle.com/chumajin/optiver-realized-eda-for-starter-version)
  - [Optiver; EDA XGBoost starter(日本語,Japanese)](https://www.kaggle.com/matsuosan/optiver-eda-xgboost-starter-japanese)
  - [【日本語/Japanese】Optiver取り組む前準備・用語の説明など](https://www.kaggle.com/takiyu/japanese-optiver)
  - [LightGBM starter with feature engineering idea](https://www.kaggle.com/tommy1028/lightgbm-starter-with-feature-engineering-idea)


## 2021/8/19
- [kaggle日記](https://zenn.dev/fkubota/articles/3d8afb0e919b555ef068)を開始<br>
- データ内容まとめ<br>
  - train: 訓練データ
    - stock_id: 株の銘柄(112種類)
    - time_id: time_id(3830) 
    - target: volatirity(10分間の合計?)


  - book_train.parquet: 予約注文の情報
    - stock_id: 株の銘柄
    - time_id: time_id ← pivot集計時のキーカラム
    - seconds_in_bucket : sec
    - bid_price1,2: 買値の希望額
    - ask_price1,2: 売値の希望額
    - bid_size1,2: 購買希望数
    - ask_size1,2: 販売希望数


  - trade_train.parquet: 取引実績の情報
    - stock_id: 株の銘柄
    - time_id: time_id
    - seconds_in_bucket: sec
    - price: 取引価格
    - size: 取引株式数
    - order_count: 取引注文数
