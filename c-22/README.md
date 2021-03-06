# なぜアジャイルな計画づくりがうまくいくのか

- 計画づくりとはプロダクト開発の全体にわたる質問に対する最適解を探る試み
    - どれくらいのリソースを投入してどれくらいのスケジュールを提供するのか
- あらゆる可能性を探ってこれらのパラメータの可能な組み合わせを検討し、可能な範囲で最高のプロダクトを提供するための作戦を練る

## 頻繁に計画を見直してる

- 頻繁な計画の見直しがプロダクト開発への回の探索を支援する
    - イテレーションが始まるたびに計画を立てる
    - リリース計画を見直す
    - 完璧な計画を立てることが不可能だと認識すれば計画を建てることによる不安を解消する
    - 立てた計画を見直すとわかっていれば完璧な計画よりも現時点で有用な計画に集中できる
- 有用な計画は正確である
- 徐々に計画の精度を高めていく
- プロジェクトナレッジとプロジェクトナレッジを計画に反映していく

## 規模の見積もりと期間の見積もりを分離している

- 規模の見積もりと期間の見積もりを一緒にしてはならない
- 作業の大きさと作業にかかる時間は相関関係にあるが、作業にかかる時間は規模以外の要素も関わってくる
- 規模の見積もりとベロシティから期間を測定する

## 複数レベルの計画を立てている

- リリース、イテレーション、今日
- 立てた計画の目的が違う
    - 今日の計画では精度がかなり高い
        - その日に完了させるタスクへのコミットメントを表現する
    - イテレーションれべるでは精度が低くなる
        - 完了させるユーザーストーリー
        - タスクの一覧
        - ユーザーストーリーの定義は完璧でない
    - リリース計画ではもっと低くなる
        - ユーザーストーリーの優先度と見積もりだけ
- チームがプロジェクトに対して複数の時間的視野を持てるということ
    - イテレーション計画は職能横断チームが緊密に連携してイテレーションという短い期間で仕事をこなすのに必要
    - リリース計画はプロジェクト全体という広い視野をカバーする
    - イテレーションだけ見ると、より遠くにあるリリースというゴールを意識しなくなるおそれ

## 計画の基準がタスクではなくフィーチャである

- アジャイルな計画の基準はプロダクト開発に必要なタスクではなく、フィーチャに焦点を当てている
- フィーチャから捉えられる
- フィーチャを開発するようにすれば開発に必要なタスクをあまり検討しなくてもよくなる
    - イテレーションの開始時点になって初めてそのフィーチャの実装について必要なすべてのタスクを洗い出す
- フィーチャを基準にすることで、チームがフィーチャに対する理解を深めていける

## 小さなストーリーがよどみない流れを作っている

- サイクルタイム：プロセスの開始から終了までにかかる時間のこと
    - チームがフィーチャに着手してからそのフィーチャがユーザーの手元に届くまでの時間
- フィーチャの開発にかかる時間が安定していないと、サイクルタイムに大きな影響をおよぼす
    - 作業単位を小さくしてそれぞれの作業をなるべく大きな大きさに揃えるのが効果的
    - 作業の見積もりは10倍以内の範囲に収める

## イテレーションが仕掛り作業を持ち越さない

- 仕掛り作業はサイクルタイムを伸ばすことにつながる
- イテレーション終了時に仕掛作業を残さない
- 新しいイテレーションでは計画を立て直す

## チーム全体を対象にトラッキングしている

- 従来的にはチームメンバー個々人をトラッキングと評価の対象としていて起こる問題
    - タスク早く終わらせると「見積もりが甘い」と責められたり
- トラッキングをチーム単位としてタスクに個人をサインアップしないようにしたり、個人単位のバーンダウンチャートを作らないようにしたり

## 不確実性を受け入れて、計画に取り組んでいる

- 見積もりと計画づくりにをアジャイルにするということは、プロジェクトの目標と開発手法の両者に、不確実性が存在することを認めるということ
- 不確実性はイテレーションごとにプロダクトに加えた新機能や変更箇所をユーザーやステークホルダーに見せることで徐々に低減させていける

## アジャイルな計画見積もりと計画づくりの12のガイドライン

- チーム全体を巻き込む
    - プロジェクトの価値を限界まで高めるにはチーム全体の参加とコミットメントが欠かせない
    - チームで共有できる責任が増えれば増えるほど、チームが共有できる成功も多くなる


- 複数レベルの計画を建てる
    - リリース計画、イテレーション計画、今日の計画それぞれ目的がある
- 不確実性はフィーチャか日付かのいずれかで表現する
    - 追加するフィーチャが決まっていないなら計画の不確実性は日付の幅で表現する
    - フィーチャは交渉できるが期日が固定されているなら提供予定のフィーチャに幅をもたせて計画の不確実性を表現する
    - 不確実性が高いのであれば、それに応じた単位で不確実性を表現すること
- 頻繁に計画を見直す
    - 新しいイテレーションを始めるタイミング
    - 計画の見直しは、プロジェクトが組織に最大限の価値を提供できるように進んでいるかどうかを評価するチャンスだと考える
- 進捗をトラッキングして情報を共有する
    - バーンダウンチャートなどで進捗をひと目で分かるグラフで共有する
- 学習することの大切さを受け入れる
    - 新しく得た知識を必ず計画に反映すること
    - 技術への理解を深めたり、チーム作業のあり方について新しい発見を重ねることで進捗速度や進め方に対する展望を調整できる
- フィーチャは適切な大きさで計画する
    - 1,2日から10日までの大きさで
    - 労力と正確さのバランスが取れる
- フィーチャを優先づけする
    - フィーチャの価値とコストだけでなく、フィーチャから得られる知識と開発することで低減するリスクも考慮に入れる
    - プロダクトナレッジやプロジェクトナレッジを深められることが明白ならば早い段階で自走すること
- 現実に即した見積もりと計画を建てる
    - 測定した実測値を根拠とすべき
    - 進捗の0%と100%の間を測定するのが難しいので、0か100で回答すべき
- ゆとりを残す
    - チームメンバー全員の時間を100%にするような計画を建てないこと
- 複数チームの連携には「移動する先読み範囲」を使う
    - チーム間で依存関係が生じるフィーチャについては予め実装するイテレーションを決めておく

## まとめ

- アジャイルな計画づくりの目的は、プロダクト開発全体の問いに対する最適な回答を見つけ出すこと
- どんなフィーチャを、どれだけのリソースで、いつまでにつくるのか
- イテレーションを繰り返しながら近づいていく
- 異なるレベルで計画を立て、頻繁に見直す
- タスクではフィーチャを基準として、まず大きさを見積もり期間を算出する
- ストーリーは小さくし、イテレーションをまたがない
- 進捗はチーム単位でトラッキングして、個人の進捗は計測しない
- 不確実性を受け入れ、計画に反映させる
