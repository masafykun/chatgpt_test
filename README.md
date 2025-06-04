# 自動売買サンプルスクリプトの利用方法

このリポジトリには、ニュースやSNSから情報を取得して自動売買を行う例として `auto_trade.py` を含みます。学習目的のサンプルであり、投資助言を行うものではありません。利用は自己責任でお願いします。

## 推奨環境

- CPU: 1GHz以上
- メモリ: 4GB以上
- OS: Linux, macOS, Windows いずれかで Python 3.9 以上が動作すること
- Pythonおよびpipがインストールされていること
- インターネット接続

## セットアップ手順

1. リポジトリをクローン
   ```bash
   git clone <このリポジトリのURL>
   cd chatgpt_test
   ```
2. 依存パッケージをインストール
   ```bash
   pip install -r requirements.txt
   ```
   最低限 `requests` が必要です。Twitter API 等を使用する場合は `tweepy` などもインストールしてください。
3. `auto_trade.py` 内の API キーを設定
   `TWITTER_BEARER_TOKEN` や `BROKER_API_KEY` などの値を自身のものに置き換えます。
4. スクリプトを実行
   ```bash
   python3 auto_trade.py
   ```

スクリプトは 1 分ごとにニュースを取得して売買判断を行います。取引ロジックはプレースホルダーなので必要に応じて実装を追加してください。

## 免責事項

本スクリプトは投資助言を目的としておらず、利用によって生じたいかなる損害に対しても、作成者は責任を負いません。
