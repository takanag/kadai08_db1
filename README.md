# ①課題番号-プロダクト名
8 源泉温泉検索「源泉しか勝たん」 管理者用「番台メニュー」

## ②課題内容（どんな作品か）
温泉のなかでも源泉は別格！ でも源泉の温泉がどこにあるのか、検索するのは至難の業。そこでみんながお気に入りの源泉情報を共有する口コミサイト。同じ源泉フリークとして、自分のお気に入りの源泉も共有しよう！

## ③DEMO
https://takanag.sakura.ne.jp/kadai08_db1/index.html

## ④作ったアプリケーション用のIDまたはPasswordがある場合
なし

## ⑤工夫した点・こだわった点
先週作成した「源泉しか勝たん」に管理者用「番台メニュー」を追加し、源泉施設情報の登録と読み込みをmySQLで実装しました。
- 登録したい源泉温泉の名前を検索すると、Google Location APIを使って候補をリストアップ
- Location APIの位置情報と紐づけて、源泉温泉の施設情報（紹介文やロケーションなど）をphpに登録
- ユーザーとして行きたい源泉温泉の名前を検索すると、Locaion APIの位置情報と紐づけて、番台メニューにて登録した源泉施設情報をphpから出力して表示

こだわった点は、
- Google Location API, Google Map Javascript APIとphpとmySQLが連携するように実装
- APIとphp間でデータをやりとりするためにjson形式でのデータ連携

## ⑥難しかった点・次回トライしたいこと(又は機能)
- ここまで機能を複雑に作り込むと生成AIは役に立たず、細かな機能のパーツ作成とバグの特定だけ利用し、各パーツを自力で繋げて動作させるようにした
- サーバー側でOpen AIを実装して、番台メニューとして源泉温泉の施設情報を登録する際に自動で入力を行えるようにする（実装したのですがうまくデータが返ってこないので今回は断念しました）

## ⑦質問・疑問・感想、シェアしたいこと等なんでも

- [参考記事]
