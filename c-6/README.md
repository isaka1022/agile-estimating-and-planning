# 見積もりの技法

- 見積もりでも収益逓減の法則が働く
    - ある程度以上の労力を費やしても、見積もりの正確さには影響しない
- 見積もりのどれだけの時間を費やすかは見積もりの目的によって変えるべき
- どれだけの労力をかけても、正確性が最大になることはない
- 最初の見積もりの正確さはわずかな労力だけで一気に向上する
- 労力をかけすぎると見積もりの正確性は低下していく
- 予算、スケジュール、スコープは事前に確定しなければならず、プロジェクトの成功を事前に決めた厳密な計画通りのフィーチャを予算通り期日に納品することとすると労力に見合った正確さが得られない
- アジャイルチームは対照的
    - 見積もりから不確定要素を取り除くことは不可能
    - 信頼のおける計画を建てられるのは、テスト済のフィーチャを少しずつ頻繁に提供するから

## チームでの見積もり

- 見積もりを出すのはチームの中で一人ではない
- 作業する当人が正確に見積もれることはよく知られている
- 見積もりをチームで出したほうが良い理由
    - アジャイルプロジェクトでは、誰がどの作業をするのか事前にはわからない
        - ほかの人が急に担当する可能性も出てくる
    - 他のメンバーがその作業に意見がある可能性がある
        - 「前に同じようなことをしたときに、こんなことがあったよ！」

## 見積もりのスケール

- 人は10倍以内のものならうまく見積もれる
- うまくいく見積もりスケール
    - 1,2,3,5,8
        - フィボナッチ数列
    - 1,2,4,8
        - 前の数値の2倍数
- 見積もりスケールの数値は、その大きさの仕事がちょうどはいるバケツ
- 見積もりに0が使えると便利なケース
    - すべてのフィーチャーのサイズを10倍以内に抑えるため
    - 作業量が1よりも0に近い作業を、ベロシティの計算対象に含めると不都合が生じるから
- 見積もりのスケールを0にした際にはステークホルダー全員の理解を得る必要がある

## ユーザーストーリー、エピック、テーマ

- 一般的にユーザーストーリーの見積もりは10倍以内の範囲で抑えるのが望ましい
    - そのためには細かく記載する必要がある
    - 大きな単位で見積もりたい大きなユーザーストーリーをエピックとよぶ
- 近い将来に実装予定のユーザーストーリーは1回のイテレーションで完了できるくらいに小さくなっている必要がある
- 着手が1イテレーション委譲先になるものはエピックやテーマのままでよい

## 見積もり技法

- 最もよく使われる見積もり技法
    - 専門家の意見
    - 対比
    - 分割

### 専門家の意見

- 専門家にきく
- アジャイルプロジェクトではあまり役に立たない
    - フィーチャはユーザーに対する価値である
    - フィーチャの開発では一人でまかないきれないような様々なスキルが必要になるから
    - 従来型のプロジェクトでは見積もり対象はタスクであり、タスクごとに担当者をわりふるから
- あまり時間はかからない

### 対比

- このストーリーはあのストーリーよりも少し大きいと考えるやり方
- 特定の喜寿でなく、今までに見積もったストーリーのいくつかと対比する
- 三角測量
    - 3ポイントのストーリーよりも大きく、8ポイントのストーリーよりも小さい

### 分割

- ストーリーやフィーチャを見積もりやすいように小さく分ける
- 分割しすぎると数が多くなって見落とす可能性もある

## プランニングポーカー

- アジャイルチームで一番うまくいくことがわかった見積もり技法が「プランニングポーカー」
- 参加者は開発者全員：プログラマ、テスタ、データベースエンジニア、アナリスト、ユーザーインタフェースデザイナ
- 参加者が10名以上いるのであれば分割した方が良い
- プランニングポーカーのゴールは、低コストで価値のある見積もりを出すこと
- プロダクトオーナーと質疑応答する
- 終わったら、各担当者ごとに同じスケールで見積もりをして同時に開示する
- 見積もりが異なるときは、高い数値の参加者と低い参加者のそれぞれに根拠を説明してもらう
    - 見積もった人を非難数量にしてはならない
- 議論は数分程度ならかまわず、終えたら再度見積もりをする

### 議論を長引かせないために

- コストをかけすぎないために、議論の時間をあら感じめ決めておく

### 小規模なセッション

- 理想はチーム全員参加だが、一部だけでもよい
- 分割されたチームのぞれぞれには3名の見積もり担当者が必要
- チームに一貫した見積もりをもたせること
    - 最初に全体で行ってそのあとにチームにわかれてすることで、最初のセッションが基準になる

### 実施のタイミング

- プロジェクトの開始前、最初のイテレーション
- イテレーションの途中で新しいストーリーを発見した場合
- いつでも封筒に入れておいて、個人がそこに手漉きで見積もりを入れる
### プランニングポーカーがうまくいく理由

- 複数の専門家の見解をまとめた見積もりを実現する
    - あらゆる分野から集められた職能横断型ちーうｍ
- 活発な対話を引き出す
- 個人の見積もりを平均したほうがよい結果を残す傾向がある
- 楽しいから

## まとめ

- 労力を増やしても見積もりが正確になるとは限らない
    - 目的の応じて決めうr
- 見積もりは作業担当者が行うのが最適
    - アジャイルでは誰が担当するかわからないのでチームで行うべき
- 見積もりは事前に決められたスケールに従って行うべき
- みつもりを出すための岐阜鬼は専門家の意見、対比、分割がある
- プランニングポーカーを使う