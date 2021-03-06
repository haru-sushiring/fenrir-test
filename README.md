# 採用課題
とある企業の新卒採用課題でWebアプリケーションを開発しました。

## アプリ名
現在地付近のレストラン情報を検索するウェブアプリ

## アプリURL
https://restaurant.sushiringblog.com/

## 対象 OS およびブラウザ(ver.含む)
※2022年7月13日現在

- macOS Monterey 12.4
- Windows10
- iOS 15.5
- Google Chrome（103.0.5060.114）
- Safari（15.5）

## 開発環境/言語
### 開発環境
- MAMP
- Sublime Text

### 言語
- HTML
- CSS
- JavaScript
- PHP

## 開発期間
2週間

## 機能概要(機能一覧)
- GPSを利用し、現在地を取得
- 検索範囲を指定できる
- 検索結果が一覧で表示される
- 最大15件調べられる
- 詳細ページ（shop.php）は、Cookieを利用して店舗情報を表示される
- スクロールして上に戻るボタン
- ページング機能

## 不具合情報
削除できないCookieが端末に登録されている場合、詳細ページ（shop.php）に店舗情報を挿入できない。  
→ Cookieを登録する際に、先頭に削除できないCookieが付いてしまい、上手くCookie情報を取り出せなかったため。  
→ シークレットモードを利用することで、不具合を回避可能。

## フレームワークなど(ver.含む)
- Bootstrap（5.0.2）
- Font Awesome（5.15.3）
- Geolocation API
- グルメサーチAPI

## テーブル定義(ER 図)などの設計ドキュメント
### 設計図
![fenrir_restaurant_設計図 (1)](https://user-images.githubusercontent.com/80729160/178891411-3d4874fb-c53f-4f37-a751-d1ee8c07eed3.jpg)

### ER図
![fenrir_restaurant_ER図](https://user-images.githubusercontent.com/80729160/178891183-0ddb4eb4-41de-4c41-abb9-7c34cac9da33.jpg)

## コンセプト
ワンクリックで近くのお店が分かる

## こだわったポイント
- 矢印ボタンを押してページが切り替わった時に、上に自動でスクロールする所。
- 検索中に「Locating…」と表示させたこと。
- 詳細ページは別タブを開いて見れるようにしたこと。
- 環境変数を利用し、API_KEYを公開しないように工夫したこと。
- 最大の表示店舗数を15件に絞り、店舗数が多すぎてユーザーを迷わせないようにした。

## デザイン面でこだわったポイント
- 店舗情報をボーダーでデザインし、影をつけた所。
- 配色は黒系と青系のみ使用し、シンプルに仕上げた所。
- タブレット以上の大きさで、見やすいように、画像と店舗情報を横並びで表示させた所。
- 全てを中央寄せにせず、適度に左寄せや右寄せを利用した所。

## アドバイスして欲しいポイント
- 詳細ページを別ダブで開かないと、検索ページに戻った際に検索やり直しになってしまう。何か良い方法はありますでしょうか。
- 画面下の「<<」「<」「>」「>>」を押すと、常に上に戻ってしまう。店舗情報を書き換えたときだけ上に戻りたい場合、技術的に可能なのでしょうか。

## 自己評価
75点

- 事前にロードマップを引いて、工程を予め考えておくと、スムーズに開発できたかもしれない。
- 前半がゆっくり過ぎて、後半に工程が多くなってしまった。
- MAMP、API、環境変数を初めて利用したが、上手く利用することができた。
- デザイン面もこだわれた。
- 期限までに完成できた。

## 改善したいこと
1. 詳細ページ（shop.php）で、お店のGoogleMapを表示させたい。
2. 検索条件を範囲だけでなく、他も利用したい。
3. Cookieではなく、MySQLなどのデータベースでも試してみたい。
4. Cookieのエラー問題を解決したい。

以上となります。
