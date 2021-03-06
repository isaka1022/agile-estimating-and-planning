- これから自動テストについて解説する上で使っていくフレームワーク・モデル・用語を解説
- 中心になるモデルは**テストのピラミッド**

# 1.1 美しかった自動テスト

- 2001年に独自に内製し、完全に自動化されたUIテストフレームワークを完成させた
    - ボタンをクリックするだけ
        - アプリケーションが起動
        - テストを記録
        - 再生して記録した動作を検証できる
        - ビルドエンジニアたちは継続的なビルドとインテグレーションのテストに組み込んでいた
        - **しかし**

# 1.2 車輪が転がるように

- 自動テストのフレームワークを使えば使うほどシステムに新しい機能を追加するのが困難になることに気づいた
    - 自動テストでカバレッジを達成しているし、変更は継続的に統合しているし、定期的にリリースしているのに、、
    - 多くの自動UIテストを書くことで開発が遅くなる理由は見つからなかった
- いくつかの阻害要素があった
    - ユニットテストを書くことをやめてしまっていた
        - ユニットテスト：高速で小さなコードベースのテスト
        - UIテストに置き換えていたため自動ビルドに長い時間がかかるようになっていた
        - テストが壊れても気づくのに時間がかかっていた
    - テストに時間がかかるので、開発者はテストを実行しなくなっていた
        - ビルド時間 10min→3hoursになっていた
    - ある日すべてが崩壊

# 1.3 3つの厳しい教訓

- 教訓
    - すべての自動テストが同等の力を持っているわけではない。あるテストをする場合に、得的の種類のテストが、他のテストよりも優れている場合がある
    - ある種類のテストを「書くことができる」というだけでは、必ずしもそのテストを「書くべき」という理由にはならない
    - スピードとフィードバックが重要。テストケースの実行に長い時間がかかるほど、開発サイクルは遅く、反復回数は少なくなる
- 自動テストが1種類でどんな場合にも通用するような万能薬ではない
    - さまざまな種類があり、それぞれがテストするものは異なっている

# 1.4 テストのピラミッドに入り込む

![スクリーンショット 2021-11-17 23.26.19.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/29e50e22-03de-4775-9a6d-72ac9f729303/スクリーンショット_2021-11-17_23.26.19.png)

- UIテストはシステム全体をエンドツーエンドで操作
    - ユーザーがシステムを使うのと同じように振る舞う
- 統合テストではユーザーインターフェイスの下の層でサービスを直接テスト
- ユニットテストは小さく、高速で、正確なコードレベルのテスト
    - 作ったものが壊れていないことをすぐ確認するために開発者が書くもの

## 1.4.1 章の順序

- 本書では上から降りていきますが、その理由は3つ
    - 素早い成功
        - UIテストは3つの中で最もやりやすく、後押ししてくれる
    - 基礎を学ぶ必要性
        - HTMLとCSSをまずは学ばないとJSは学べない
    - 深い学習
        - 筆者はときどき読者をミスリードします
        - いいと見えたものを後から失敗させることで深い学習させる
- 章の順番は関係ないが、上から始めることで楽しく深く学べます

## 1.4.2 3つの層

- UI層
    - 顧客が操作するボタンなど
- サービス層
    - UI層の表示を更新するのに必要なデータを提供
- ロジック層
    - 計算、演算、処理の根幹
- このようなアプリケーションの各層がピラミッドの層に対応する

# 1.5 UIテスト

- UIテストはアーキテクチャのすべての層を通過し、すべてがつながっていることを保証
- 問題はスピードと壊れやすさ
- ユニットテストに比べてスピードが桁違いに遅いという事実に対しての回避策はない
- 多くは使われない理由

# 1.6 統合テスト

- 統合テストは複数の層がつながっていることを確認する機能を保ったまま、UIの壊れやすさにも影響しない
- 欠点はそれほど詳細ではないこと
- 何かが壊れていることはわかっても、どこが壊れているかまではわからない

# 1.7 ユニットテスト

- 正確性、スピード、カバレッジにおいて頼りになるのはユニットテスト
- 自動テストの父
- 唯一の欠点は統合部分
    - 全体がつながっているかという観点では見落としをすることがある

# 1.8 親指の法則

- 自動テストの大部分は底辺に近い層で行うほうが良い
    - 上の層にいけばいくほど低速でコストが高くなる
- すべてのプロジェクトがUIを操作するテストを必要としているわけではない
- システムに新しいてs津をお追加するときには、下の層から始めて、上の層に上がっていくようにします
- **新しいテストを追加するときには、常に「ユニットテストでカバーできないか」を最初に確認しよう**
- **常に、テストをできる限りピラミッドの下の層に入れること**
- **すべてを自動化しようとしないこと。代わりに、過不足なく自動化しよう**
- ところが、上にあるテストは常に下の層のテストの上位集合なので、同じ機能をテストしてりうという意味では部分的な重複は避けられない
- ユニットテストとUIテストの違い
- ユニットテストを書く場合
    - 設計を正しく反映できているか？
    - 最後の変更でなにか壊していないか？
    - 私達の想定と特殊なケースはすべて整合性が取れているか？
    - 新しい機能を追加することは安全か？
- テストの糸が重複しているのでなければ、機能面の重複は全く問題がない

# 1.9 誰が自動テストを書くのか

- 専門分野が異なるチームが協働する場合、誰が何をすべきなのか明らかにする
- 開発者は自動テストはスピードがすべて
    - どこが壊れたのか迅速なフィードバックを求める
- テスターは正確さ、幅広さ、深さがすべて
- 開始時点での状態

- 正解はないが、うまく進めるための方法
    - テスターの多くはUIテストと統合テストに取り組む
    - 開発者はユニットテストに夢中になる
- どのようなやり方をするにしても、協力して一緒に動くことが大事
    - テスター：開発者のいたポジションに飛び込んで、テストの自動化について大きな範囲を担当しよう
    - 開発者：テスターの生産性を上げることに関心を持とう

## 探索的テストを忘れないこと

- 探索的テストとは、手順化されておらず、網羅的にアプリケーションを操作して不具合を見つけるようにするテスト
    - 自動テストでは見つからない問題を見つけることも
- 自動テストスイートを手に入れたら、立ち戻って探索的テストをを続けることも忘れないで
