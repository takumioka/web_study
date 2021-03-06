# 第一回勉強会
## 1-1 WEBとは
 ```
 Webとは、インターネット上で標準的に用いられている、文書の公開・閲覧システム。文字や画像、動画などを一体化した文書を  
 ネット上で公開・配布したり、また、それを入手・閲覧することができる。文書内に別の文書への参照を埋め込むことができる  
 「ハイパーテキスト」と呼ばれるシステムの一種。“web”とは蜘蛛の巣の意味であり、大規模なハイパーテキストの文書間の繋がりを  
 図示すると複雑な蜘蛛の巣のように見えることからこのように呼ばれる。
 ```
 ## 1-2 webを支える技術
 ### HTTPとは
 * 通信プロトコル ホームページでデータを受け渡しするために使う  
 
 * HTTPはTCP/IPをベースにしている  
![TCP/IPの説明 ](https://www.infraexpert.com/studygif/tcpip2.gif)
### クライアントとサーバー

* クライアント (WEBブラウザー)  
    ** サーバーに接続して各種リクエストを要求しレスポンスを受け取る
* サーバー(WEBサーバー)  
    ** 要求されたリクエストを処理してクライアントに返す
![クライアントとサーバーの説明 ](https://image.jimcdn.com/app/cms/image/transf/none/path/s1fa74a0f1ede5508/image/ic24ffc5420bd079f/version/1469493659/image.png)
### ステートレスとステートフル
ステートレス
```
ステートレスとは、システムが現在の状態を表すデータなどを保持せず、入力の内容によってのみ出力が決定される方式。同じ入力に対する出力は常に同じになる。
```
ステートフル
```
ステートフルとは、システムが現在の状態を表すデータなどを保持しており、その内容を処理に反映させる方式。同じ入力に対する出力が常に同じとは限らず、内部の状態次第で変わることがある。
```
* httpはステートレスなプロトコル

[参照 ステートフル(Stateful)とステートレス(Stateless)の違い](https://milestone-of-se.nesuke.com/nw-basic/as-nw-engineer/stateful-and-stateless/)

### HTTPメゾット
httpメゾットとは
  ```
   データのやり取りをする際のお願いするためのもの
  「GET」とか「POST」とかのこと
  ```
  * httpメゾットの種類

|メゾット|意味|
|:--|--:|
|GET|リソースの取得|
|POST|子リソースの作成、リソースへのデータ追加、その他処理|
|PUT|リソースの更新、リソースの作成|
|DELETE|リソースの削除|
|HEAD|リソースのヘッダ (メタデータの取得)|
|OPTIONS|リソースがサポートしているメソッドの取得|
|TRACE|プロキシ動作の確認|
|CONNECT|プロキシ動作のトンネル接続への変更|

* この4つだけ覚えればいい  
  GET,POST,PUT,DELETE  
  * 理由   
　　CRUDの性質を満たすため  
    * CRUDとはCreate(作成),Read(読み込み),Updaate(更新),Delete(削除)というデータ操作の4つの処理のこと
  
[もっと知りたい場合のリンク](https://qiita.com/Ryutaro/items/a9e8d18467fe3e04068e)

[自分がまとめたやつより100倍わかりやすい記事](https://qiita.com/7968/items/4bf4d6f28284146c288f)

