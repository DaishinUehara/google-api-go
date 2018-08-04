# google-api-goの利用サンプル

## 前提条件

すでにGCPにアカウントがあることを前提としています。
もし無料枠でいろいろやりたいときには以下を参考にしましょう。  

[GCE の無料枠のサーバを立るときに、初見でハマりそうなところ][2]

## 手順

以下のサイトをもとに記載しています。  
[GOOGLE COLUD PLATFORM での GO][1]

    go get -u cloud.google.com/go/storage

[GOOGLE COLUD PLATFORM での GO][1]リンクの「ENABLE THE API」のボタンを押下。

Google Cloud Platform の プロジェクトの選択で対象プロジェクトを選択し「続行」ボタンを押下する。  
これにより「Google Cloud Strage JSON API」が有効になる。

### Google App Engine または Computing Engineで APIを用いる場合

「認証情報に進む」のボタンを押下する。

「プロジェクトへの認証譲歩の追加」画面で「App EndgineまたはComputing EngineでこのAPIを利用する予定はありますか？」で「はい」を選択し「必要な認証情報」を押下。

「必要な認証情報」を押下。

「Google Cloud Storage JSON API を ウェブサーバー から呼び出します」が表示され
「完了」を押下する。これを選択すると「Google Compute Engine」か
「Google App Engine」からAPIを呼び出すことになる。

### Google App Engine や Computing Engine 以外から APIを用いる場合

#### API キー、クライアント ID、サービスアカウントを作成する



#### OAuthを用いる

[1]:https://cloud.google.com/go/home?hl=ja
[2]:https://qiita.com/ndxbn/items/7ef0a96e409a5b5837bd
