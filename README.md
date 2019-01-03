# Portfolio Game

- 全体的に可愛い感じにしたい
- 参考イメージは今後Pintarestを中心に集めていく
  - [Pinterest](https://www.pinterest.jp/mihoijuin/%E3%83%9D%E3%83%BC%E3%83%88%E3%83%95%E3%82%A9%E3%83%AA%E3%82%AA%E3%82%A2%E3%82%A4%E3%83%87%E3%82%A2/)

## ざっくり要件（2019/01/03時点）
### WEB上
- PCのみに対応し、スマホからアクセスされたら別画面を見せる
- ヘッダーにはサイトタイトル、フッターにはコピーライトのみのせる
- タイトルロゴはいい感じのにしたい
- プレイ方法などのゲームの説明ははWebGLの上方のWeb画面に書く
- [vue-unity-webgl](https://www.npmjs.com/package/vue-unity-webgl)を使用する
  - 参考：[Unityで吐いたWebGLをPWAで動かしてみた - Qiita](https://qiita.com/MizoTake/items/7089494d7bd3e700e34b)
- デプロイはfirebaseを使う
- 独自ドメインを取ってみたい
- [unityroom](https://unityroom.com/)にも投稿したい
- ただし今回Webはメインではないのでそこまでこだわらない
- ゲーム部分がひと段落したらJavascriptの練習台にするのはアリ

### ゲーム
- ゲーム風にスタート画面があり、スタートボタンを押すと始まる
- キャラクター画面と探索画面がある（シーンはこの2つ
- キャラクター画面ではポートフォリオ的な説明が見れる場所だが、はじめキャラが浮かんでるだけ
- 探索画面で探索するとプロフィールに関連するアイテムを発見できる
- アイテムを発見するたびにキャラクター画面が完成されてく（できればキャラクターも最初は卵とかで、見つけるたびに進化するとかだと楽しい）
- 見つかるとキャラクター画面へのボタンが何かしら反応するのが良い
- キャラクター画面の最終コンテンツはこのページの内容の簡略版：[Porin - Porin's Room](https://scrapbox.io/Porin-Room/Porin)
- プロフィール関連アイテムあんまり多すぎるとつらいので5、6個くらい？（どうやって見つけられるかでセンスが試される...）
  - 経歴
  - SNSなどへのリンク
  - スキル
  - 作ったもの
  - 好きなこと
  - 苦手なこと

## ゲーム開発方針
### プロト
- 動きだけ再現
- デザインや演出は無視
- 探索画面でアイテムをゲット→キャラクター画面の表示が変わる
  - アイテムのゲット方法は接触+アイテムクリックで試そう
- スタート画面は用意する
- スタート後、データ状況によって表示を変える（取得済みアイテムは表示しないなど）
- 使いまわせるようになるべくメソッド化、Prefab化しておく

### デザイン
- Pintarestを参考にしながら簡単なもので作る
- アイテム発見方法、キャラクター画面の変化パターンなどもここで決める
- アニメーションはまだ考えない

### アニメーション
- デザインを実装したら考える
- ここはこだわったらどんどんこだわれるので、いろんな演出を試して練習したい
- 演出によっては新しく素材を足す場合もありそう