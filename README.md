# Data Science

データサイエンスに関する内容をPythonをベースにまとめていきます。

## Setup

#### Requirements

下記の環境を用意してください。

- Python3.5
- Jupyter Notebook
- Numpy
- Scipy
- Pandas
- seaborn / matplotlib
- Scikit-learn

バージョンを合わせたい場合は下記のようにコマンドを入力してください。

```
$ python3.5 -m venv venv
$ source venv/bin/activate
$ pip install -r requirements.txt -c constraints.txt
```


#### Setup with Docker

Dockerが使える場合は、簡単に環境を用意することができます。
jupyter notebookは[公式でdocker imageを公開](https://github.com/jupyter/docker-stacks/tree/master/datascience-notebook) しているので、そちらを利用しましょう。

```
$ docker pull jupyter/datascience-notebook
$ docker run -p 8888:8888 -v $PWD/notebooks:/home/jovyan/work jupyter/datascience-notebook
```

pandas-validatorやoutlier-utilsを使いたい場合は、このRepositoryにおいてあるDockerfileを使ってください。

```
$ docker build -t c-bata/datascience .
$ docker run -p 8888:8888 -v $PWD/notebooks:/home/jovyan/work c-bata/datascience
```


## Contents

追加予定のコンテンツ一覧です。

#### データ加工(Data Wrangling)・可視化

- Pandasの基礎
- 異常値・外れ値・欠損値
- 可視化(matplotlib, seaborn)

#### 統計(Statistics)と機械学習(Machine Learning)

- 機械学習の基礎知識
- 回帰分析
- 決定木
- クラスタリング
- パターン認識
- パラメータ推定
- アンサンブル学習
- 分類器

