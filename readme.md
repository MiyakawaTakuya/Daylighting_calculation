# 採光計算ツール(建築基準法 住宅 住居系地域限定ver)
建築を計画する際に採光の計算を行うが、それを簡単にするための補助的なツール
(３時間くらいで作ったのでホントに簡易的なもの)

#### 詰まってしまって中断した案件
### GitHubの草を集めて視覚的に表現し、エンジニアマインドに火をつけてモチベーションを維持する装置

## 方法
方法1：GitHubページをスクレイピングし草の数値データと日付を取得。
HTMLを文字列で抽出 
→正規表現で欲しいデータをピンポイントで得る
→DBに入力する(ユーザー、日付、日の数値、月の数値、全体の数値etc)
→リードでHTMLに落とす
→p5.jsなどを使いながら死角に訴えかける表現にする

方法２：GraphiQLを使ってGitHubのGraphQL APIを触り、数値データと日付を取得。アクセストークンの作成する。クライアントとしてGraphiQL.appをインストール、起動させる.
→その後の流れはほとんど同じ想定

## 結果と反省
方法１はなかなか文字列化するのが上手くいかず途中で断念、方法２は文字列化まで行ったもののPHPのInputをあまり活用できてないと思い中断.
・PHPを使わずapp経由でcontributionsを取得できてしまうため、今回の課題の趣旨からずれてしまった
・GitHubでアクセストークンが必要となり、承諾をもらえた相手しか表示できない.