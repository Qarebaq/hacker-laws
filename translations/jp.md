# 💻📖 ハッカーの法則

開発者が役に立つと思う法則、理論、原則、パターン。

[翻訳](#翻訳): [🇧🇷](./translations/pt-BR.md) [🇨🇳](https://github.com/nusr/hacker-laws-zh) [🇫🇷](./translations/fr.md) [🇮🇹](./translations/it-IT.md) [🇱🇻](./translations/lv.md) [🇰🇷](https://github.com/codeanddonuts/hacker-laws-kr) [🇷🇺](https://github.com/solarrust/hacker-laws) [🇪🇸](./translations/es-ES.md) [🇹🇷](./translations/tr.md) [🇮🇩](./translations/id.md) [🇵🇱](./translations/pl.md) [🇻🇳](./translations/vi.md)

このプロジェクトが気に入りましたか？ぜひ私と[翻訳者](#%E7%BF%BB%E8%A8%B3)を支援すること[ご検討ください。](https://github.com/sponsors/dwmkerr)

---

<!-- vim-markdown-toc GFM -->

- [イントロダクション](#イントロダクション)
- [法則](#法則)
    - [90-9-1 原則(1％ルール)](#90-9-1-原則1ルール)
    - [アムダールの法則](#アムダールの法則)
    - [割れ窓理論](#割れ窓理論)
    - [ブルックスの法則](#ブルックスの法則)
    - [コンウェイの法則](#コンウェイの法則)
    - [カニンガムの法則](#カニンガムの法則)
    - [ダンバー数](#ダンバー数)
    - [ゴールの法則](#ゴールの法則)
    - [グッドハートの法則](#グッドハートの法則)
    - [ハンロンの剃刀](#ハンロンの剃刀)
    - [ホフスタッターの法則](#ホフスタッターの法則)
    - [ハーバーの法則](#ハーバーの法則)
    - [ハイプサイクルとアマラの法則](#ハイプサイクルとアマラの法則)
    - [ハイラムの法則（暗黙のインターフェースの法則）](#ハイラムの法則暗黙のインターフェースの法則)
    - [カーニガンの法則](#カーニガンの法則)
    - [リーナスの法則](#リーナスの法則)
    - [メトカーフの法則](#メトカーフの法則)
    - [ムーアの法則](#ムーアの法則)
    - [マーフィーの法則/ソッドの法則](#マーフィーの法則ソッドの法則)
    - [オッカムの剃刀](#オッカムの剃刀)
    - [パーキンソンの法則](#パーキンソンの法則)
    - [早すぎる最適化](#早すぎる最適化)
    - [パットの法則](#パットの法則)
    - [リードの法則](#リードの法則)
    - [複雑性保存の法則（テスラーの法則）](#複雑性保存の法則テスラーの法則)
    - [漏れのある抽象化の法則](#漏れのある抽象化の法則)
    - [パーキンソンの凡俗法則](#パーキンソンの凡俗法則)
    - [UNIX哲学](#unix哲学)
    - [Spotifyモデル](#spotifyモデル)
    - [ワドラーの法則](#ワドラーの法則)
    - [ウィートンの法則](ウィートンの法則)
- [原則](#原則)
    - [ディルバートの原理](#ディルバートの原理)
    - [パレート原理（80/20ルール）](#パレート原理8020ルール)
    - [ピーターの原則](#ピーターの原則)
    - [堅牢性の原則（ポステルの法則）](#堅牢性の原則ポステルの法則)
    - [SOLID](#solid)
    - [単一責任の原則](#単一責任の原則)
    - [開放/閉鎖原則](#開放閉鎖原則)
    - [リスコフ代替原則](#リスコフの置換原則)
    - [インターフェース分離の原則](#インターフェース分離の原則)
    - [依存関係の逆転の原則](#依存性逆転の原則)
    - [DRY原則](#dry原則)
    - [KISS原則](#kissの原則)
    - [YAGNI](#yagni)
    - [分散コンピューティングの落とし穴](#分散コンピューティングの落とし穴)
- [関連書籍](#関連書籍)
- [翻訳](#翻訳)
- [関連プロジェクト](#関連プロジェクト)
- [貢献方法](#貢献方法)
- [TODO](#todo)

<!-- vim-markdown-toc -->

## イントロダクション

ソフトウェア開発の話をするときに話題にのぼる法則はたくさんありますよね。このレポジトリでは、その中でも最も一般的なものをリストアップしその概要を説明しています。ぜひ、シェアしたりプルリクエストしてください!

❗: このリポジトリには、いくつかの法則や原則、パターンの説明が含まれていますが、このレポジトリはそれらを*推奨*するものではありません。適用すべきかどうかは、常に議論の余地がありますし、あなたが何に取り組んでいるかに大きく依存します。

## 法則

そして、ここからが本編!

### 90-9-1 原則(1％ルール)

[1%の法則-Wikipedia](https://ja.wikipedia.org/wiki/1%25%E3%81%AE%E6%B3%95%E5%89%87)

90-9-1原則は、wikiのようなインターネットコミュニティ内では、参加者のうちコンテンツを閲覧しているだけの人が90%、コンテンツを編集や修正する人が9%、残りの1%がコンテンツを追加することを示唆しています。

実際の例:

- 4つのデジタルヘルスソーシャルネットワークの2014年の調査によると、上位1％が投稿の73％を作成し、次の9％が平均約25％の投稿を作成し、残りの90％が平均2％を作成するという結果が示されてます。（ [参考文献](https://www.jmir.org/2014/2/e33/) ）

関連項目：

- [パレートの法則](#パレート原理8020ルール)

### アムダールの法則

[アムダールの法則-Wikipedia](https://ja.wikipedia.org/wiki/%E3%82%A2%E3%83%A0%E3%83%80%E3%83%BC%E3%83%AB%E3%81%AE%E6%B3%95%E5%89%87)

> アムダールの法則とは、リソースを追加した場合に、*期待できる性能向上*の程度です。通常、並列コンピューティングで使用され、プログラムの並列性によって制限されるプロセッサの数を増やすことによる実際の利益を予測することができます。

例を挙げて説明します。プログラムが、1つのプロセッサで実行されなければならないパートAと、並列化できるパートBの2つのパートで構成されている場合、プログラムを実行するシステムに複数のプロセッサを追加しても、限られた利益しか得られないことがわかります。パートBの速度を大幅に向上させることは可能ですが、パートAの速度は変わらないでしょう。

下記の図は、並列度増加と期待する速度改善の例を示しています。

<img width="480px" alt="Diagram: Amdahl's Law" src="../images/amdahls_law.png">

*（画像参照：英語版ウィキペディアのDaniels220、クリエイティブコモンズの表示-継承3.0非移植、https：//en.wikipedia.org/wiki/File：AmdahlsLaw.svg）*

このように、50%の並列化が可能なプログラムであっても、10個の演算処理装置を超えるとほとんど恩恵を受けませんが、95%の並列化が可能なプログラムであれば、1000個以上の演算処理装置でも大幅な速度向上を達成することができます。

[ムーアの法則](#ムーアの法則)による性能向上が鈍化し、個々のプロセッサの処理速度の進化が遅くなると、並列化が性能向上の鍵となります。最新のシェーダベースのコンピューティングでは、個々のピクセルやフラグメントを並列にレンダリングすることができます。現代のグラフィックカードが何千もの処理コア（GPUやシェーダユニット）が搭載されている場合多い理由はこれです。

関連項目：

- [ブルックスの法則](#ブルックスの法則)
- [ムーアの法則](#ムーアの法則)

### 割れ窓理論

[割れ窓理論-Wikipedia](https://ja.wikipedia.org/wiki/%E5%89%B2%E3%82%8C%E7%AA%93%E7%90%86%E8%AB%96)

割れ窓理論は、目に見える犯罪の兆候（または環境整備の欠如）が、さらに深刻な犯罪（または環境のさらなる悪化）につながることを示唆しています。

この理論はソフトウェア開発に応用されており、質の低いコード(または [技術的負債](#TODO))は、品質を向上させる努力を無視したり、過小評価したりするという認識につながり、その結果、さらに質の低いコードの生産につながることを示唆しています。この効果は、時間の経過とともに品質を大きく低下させることにつながります。

関連項目:

- [技術的負債](#TODO)

例：

- [実用的なプログラミング：ソフトウェアエントロピー](https://pragprog.com/the-pragmatic-programmer/extracts/software-entropy)
- [コーディングホラー：割れ窓理論](https://blog.codinghorror.com/the-broken-window-theory/)
- [オープンソース：プログラミングの喜び-割れ窓理論](https://opensourceforu.com/2011/05/joy-of-programming-broken-window-theory/)

### ブルックスの法則

[ブルックスの法則-Wikipedia](https://ja.wikipedia.org/wiki/%E3%83%96%E3%83%AB%E3%83%83%E3%82%AF%E3%82%B9%E3%81%AE%E6%B3%95%E5%89%87)

> 遅延しているソフトウェア開発プロジェクトに人材を追加するとプロジェクトがさらに遅延する。

この法則は、多くの場合、すでに遅れているプロジェクトを挽回させようとして、人的リソースを追加することで、プロジェクトが更に遅延することを示唆しています。ブルックスは、これが単純化しすぎであることを明らかにしていますが、一般的な推論としては、新しい人的リソースの立ち上げにかかる時間とコミュニケーションのオーバーヘッドを考えると、短期的には速度が低下するということです。また、多くのタスクは分割出来ないことがあり、リソース間で簡単にタスク分散されない可能性があり、期待するベロシティも得られなくなることを意味します。

出産でよく言われる「9人の女性は1ヶ月で子作りができない」という言葉は、ブルックスの法則、特にある種のタスクは分割や並列化できないという事実に関連しています。

これは、「 [人月の神話](#関連書籍) 」という本の中心的なテーマです。

関連項目:

- [デスマーチ](#todo)
- [関連書籍：人月の神話](#関連書籍)

### コンウェイの法則

[コンウェイの法則 Wikipedia(英語版)](https://en.wikipedia.org/wiki/Conway%27s_law)

この法則は、システムの技術的な境界線が組織の構造を反映することを示唆しています。組織の改善を検討する際によく参考にされますが、コンウェイの法則では、組織が多くの小さな切り離されたユニットに構造化されている場合、その組織が生成するソフトウェアも小さな切り離されたユニットに構造になること示唆しています。もし組織が機能やサービスを中心とした「縦割り」に構築されているならば、ソフトウェアシステムもこれを反映し縦割りになります。

関連項目:

- [Spotifyモデル](#spotifyモデル)

### カニンガムの法則

[カニンガムの法則 - Meta - Meta-Wiki - Wikimedia](https://meta.wikimedia.org/wiki/Cunningham%27s_Law/ja)

> インターネット上で正解を得るための最良の方法は、質問をすることではなく、間違った答えを投稿することです。

スティーブン・マクゲディによると、1980年代初頭にウォード・カニンガム氏が彼にこうアドバイスをしたそうです。「インターネットで正しい答えを得る最善の方法は、質問をすることではなく、間違った答えを投稿することだ」と。マクギーディはこれをカニンガムの法則と呼んでいますが、カニンガムはこの法則の所有権を否定しており、カニンガムはこれを「誤引用」と言っています。元々はUsenet上でのやりとりのこと指していたが、この法則は他のオンラインコミュニティ（例：Wikipedia、Reddit、Twitter、Facebook）の仕組みを説明するために使われてきました。

関連項目:

- [XKCD 386：「デューティコール」](https://xkcd.com/386/)

### ダンバー数

[ダンバー数-Wikipedia](https://ja.wikipedia.org/wiki/%E3%83%80%E3%83%B3%E3%83%90%E3%83%BC%E6%95%B0)

「ダンバーの数は、安定した社会的関係を維持できる人の数に対する認知的制限の提案です。つまり、個人が各人が誰であるか、そして各個人と他のすべての人との関係を知っている関係です。」正確な数にはいくつかの意見の相違があります。 「... [ダンバー]は、人間が快適に維持できるのは150人の安定した関係だけであると提案しました。 "彼はその数をより社会的なコンテキストで説明しています、「もしあなたがバーで偶然出会って、その場で突然一緒に酒を飲むことになったとしても、気まずさを感じない人数」。この数は一般的に100人から250人と言われています。

個人間の安定した関係と同様に、コードベースと開発者の関係を維持するには努力が必要です。大規模で複雑なプロジェクトに直面したとき、や多くのプロジェクトをかかえているとき、私たちは慣例やポリシー、モデル化された手順に頼ってスケールアップを図っています。ダンバーの数字は、オフィスが大きくなったときに心に留めておくことが重要であるだけでなく、チームの責任範囲を設定したり、システムがモデリングや理論的オーバーヘッドの自動化を支援するツールにいつ投資すべきかを決定するときにも重要です。この数字をエンジニアリングのコンテキストに当てはめると、オンコールローテーションに参加してサポートすることに自信を持てるプロジェクトの数（または単一プロジェクトの複雑さを正規化した数）です。

関連項目:

- [コンウェイの法則](#コンウェイの法則)

### ゴールの法則

[ゴールの法則-Wikipedia](https://ja.wikipedia.org/wiki/%E3%82%B4%E3%83%BC%E3%83%AB%E3%81%AE%E6%B3%95%E5%89%87)

> 動作する複雑なシステムは、必ず、動作していた単純なシステムから進化したものであることがわかります。ゼロから設計された複雑なシステムは決して動作しませんし、それを動作させるためにパッチを当てることもできません。機能するシンプルなシステムからやり直さなければなりません。
> ([ジョン・ゴール(英語)](https://en.wikipedia.org/wiki/John_Gall_(author)))

ゴール法則は、高度に複雑なシステムを*設計*しようとする試みが失敗する可能性が高いことを示唆している。高度に複雑なシステムが一度に構築されることはめったになく、より単純なシステムから進化するものです。

典型的な例は、world-wide-webです。今日では、これは高度に複雑なシステムですが、しかし、当初は学術機関間でコンテンツを共有するためのシンプルな方法として定義されていました。その目標を達成することに成功し、時間の経過とともにより複雑なものへと進化していきました。

関連項目:

- [KISS (Keep It Simple, Stupid)](#kissの原則)

### グッドハートの法則

[グッドハートの法則-Wikipedia(英語版)](https://en.wikipedia.org/wiki/Goodhart's_law)

> 観察されたどのような統計的規則性も、管理する目的で圧力をかけると崩壊してしまう傾向があります。
> *チャールズ・グッドハート*

次のようにも一般的に参照されます：

> 計測結果が目標になると、その計測自体が役に立たなくなります。
> *マリリン・ストラザーン*

この法則は、測定主導の最適化が測定結果自体の価値を下げることにつながる可能性があると述べています。プロセスに盲目的に適用された過度に選択的な一連の（ [KPI](https://en.wikipedia.org/wiki/Performance_indicator) ）は、歪んだ効果をもたらします。人々は、自分たちの行動の全体的な結果に注意を払うのではなく、特定のメトリックを満たすためにシステムを「ゲーム」することで部分的に最適化する傾向があります。

実際の例：

- 十分にテストされたソフトウェアを作成することがコードカバレッジ測定の意図であったにもかかわらず、アサートなしのテストはコードカバレッジの基準を満たしています。
- コミットされた行数によって開発者を評価するとは、無駄に肥大化したコードベースを作成することに繋がります。

関連項目:

- [グッドハートの法則：間違ったものを測定することが不道徳な行動をどのように促進するか](https://coffeeandjunk.com/goodharts-campbells-law/)
- [バグのないソフトウェアのディルバート](https://dilbert.com/strip/1995-11-13)

### ハンロンの剃刀

[ハンロンの剃刀-Wikipedia](https://ja.wikipedia.org/wiki/%E3%83%8F%E3%83%B3%E3%83%AD%E3%83%B3%E3%81%AE%E5%89%83%E5%88%80)

> 無能で十分説明されることに悪意を見出すな。
> ロバート・J・ハンロン

この原則は、ネガティブな結果をもたらす行動は悪意の結果ではないことを示唆している。むしろネガティブな結果はそれらの行為や影響が完全に理解されていなかったことに起因する可能性が高い。

### ホフスタッターの法則

[ホフスタッターの法則-Wikipedia](https://ja.wikipedia.org/wiki/%E3%83%80%E3%82%B0%E3%83%A9%E3%82%B9%E3%83%BB%E3%83%9B%E3%83%95%E3%82%B9%E3%82%BF%E3%83%83%E3%82%BF%E3%83%BC#%E3%83%9B%E3%83%95%E3%82%B9%E3%82%BF%E3%83%83%E3%82%BF%E3%83%BC%E3%81%AE%E6%B3%95%E5%89%87)

> ホフスタッターの法則を考慮しても、いつも予想以上に時間がかかる。
> （ダグラスホフスタッター）

何かがどれくらいかかるかの見積もりを見るときに、この法則を聞いたことがあるかもしれません。ソフトウェア開発においては、納品にかかる時間を正確に見積もるのは人々はあまり得意ではない傾向にあります。

これは「 [ゲーデル、エッシャー、バッハ：永遠の金色の三つ編み](#関連書籍) 」という本からの引用です。

関連項目:

- [関連書籍： ゲーデル、エッシャー、バッハ：永遠の金色の三つ編み](#関連書籍)

### ハーバーの法則

[ハーバーの法則Wikipedia(英語版)](https://en.wikipedia.org/wiki/Hutber%27s_law)

> 改善とは劣化を意味します。
> （ [パトリックハットバー-Wikipedia(英語版)](https://en.wikipedia.org/wiki/Patrick_Hutber) ）

この法則は、システムを改善しようとして、他の部分の劣化につながったり、または他の劣化を隠し、全体的にシステムが現在の状態から劣化につながることを示唆しています。

例えば、特定のエンドポイントに対する応答遅延を減少させようとして、リクエストフローのさらに後フェーズのスループットやキャパシティの問題を増加させ、全く関係ないサブシステムに影響を与える可能性があります。

### ハイプ・サイクルとアマラの法則

[ハイプ・サイクル- Wikipedia](https://ja.wikipedia.org/wiki/%E3%83%8F%E3%82%A4%E3%83%97%E3%83%BB%E3%82%B5%E3%82%A4%E3%82%AF%E3%83%AB)

> テクノロジーの効果を短期的には過大評価し、長期的には過小評価する傾向がある。
> （ロイ・アマラ）

ハイプ・サイクルは、元々はガートナー社によって作成された、時間をかけてテクノロジーの興奮と発展を視覚的に表現したものです。視覚的に表示するのが最適です。

![The Hype Cycle](../images/gartner_hype_cycle.png)

*（画像参照：英語版ウィキペディアのJeremykemp著、CC BY-SA 3.0、https：//commons.wikimedia.org/w/index.php？curid = 10547051）*

要するに、このサイクルは、一般的に新技術とその潜在的な影響力について興奮があることを示唆している。チームはしばしばこれらのテクノロジーにすぐに飛びつき、その結果に失望してしまうことがあります。これは、テクノロジーがまだ十分に成熟していなかったり、実世界でのアプリケーションがまだ十分に実現されていないからかもしれません。ある程度の時間が経つと、テクノロジーの能力が向上し、実際に使用する機会が増え、チームはようやく生産性を高めることができます。Roy Amaraのこの言葉は、このことを最も簡潔に要約しています。「私たちは、テクノロジーの効果を短期的には過大評価し、長期的には過小評価する傾向がある」。

### ハイラムの法則（暗黙のインターフェースの法則）

[ハイラムの法則(英語)](http://www.hyrumslaw.com/)

> あるAPIに十分なユーザー数がいれば、契約で何を約束するかどうかは問題ではありません。 あなたのシステムのすべての観測可能な動作は、誰かに依存されることになります。
> （ハイラム・ライト）

ハイラムの法則では、APIの*ユーザ数が十分に多い*場合、APIのすべての動作(公的契約の一部として定義されていないものであっても)は、最終的に誰かに依存されるようになるということを述べています。些細な例としては、APIの応答時間などの非機能要件が挙げられます。もっと微妙な例は、APIのエラーの*タイプ*を判断するために、エラーメッセージに正規表現を適用することに依存しているユーザかもしれません。API の公開契約ではメッセージの内容について何も記述されておらず、ユーザーがメッセージではなくエラーコードを使用すべきでと明示していたとしても、*一部の*ユーザーがそれを無視してメッセージを使用する可能性があり、メッセージを変更することでそのようなユーザーのための API が本質的に壊れてしまうことになります。

関連項目:

- [漏れのある抽象化の法則](#漏れのある抽象化の法則)
- [XKCD 1172](https://xkcd.com/1172/)

### カーニガンの法則

> デバッギングはコーディングよりも2倍難しい。従って、あなたが可能な限り賢くコードを書くとしたら、定義からして、あなたはそれをデバッグできるほど賢くない。
> （ブライアン・カーニハン）

カーニガンの法則は、 [ブライアンカーニハンに](https://en.wikipedia.org/wiki/Brian_Kernighan)ちなんで名付けられ、カーニハンとプラウガーの著書[「Elements of Programming Style](https://en.wikipedia.org/wiki/The_Elements_of_Programming_Style) 」からの引用に基づいています。

> デバッグは、そもそもプログラムを書くことの2倍大変だということは誰もが知っています。では、コードを書いた時に同じくらい賢いとしたら、どうやってデバッグするのでしょうか？

双曲線的ではありますが、カーニガンの法則は、複雑なコードで発生した問題をデバッグするのはコストがかかるか、実現不可能な場合があるため、単純なコードは複雑なコードよりも優先されるべきであるということを言っています。

関連項目:

- [KISSの原則](#kissの原則)
- [UNIX哲学](#unix哲学)
- [オッカムのかみそり](#オッカムの剃刀)

### リーナスの法則

[リーナスの法則-Wikipedia](https://ja.wikipedia.org/wiki/%E3%83%AA%E3%83%BC%E3%83%8A%E3%82%B9%E3%81%AE%E6%B3%95%E5%89%87)

> 十分な目ん玉があれば、全てのバグは洗い出される。
>
> _エリック・S・レイモンド_

この法則は簡単に言うと、あるプログラムを見る人が多ければ多いほど、誰かがその問題を以前に見て解決している可能性が高くなる、あるいはそれに非常に近い状況になる、というものです。

元々はプロジェクトのオープンソースモデルの価値を説明するために使われましたが、どんなソフトウェアプロジェクトにも当てはまります。プロセスにも拡大して適用できます。より多くのコードレビューや静的解析、また多角的なテストプロセスによって、問題をより可視化されて識別しやすくなります。

より格式ばって言うと以下のようになります。

> ベータテスターと共同開発者が十分多くいれば、ほとんど全ての問題はすぐに明確になり、似た問題に以前遭遇したことのある人によって解決されるだろう。

この法則は、エリック・S・レイモンドの著作『[伽藍とバザール](https://ja.wikipedia.org/wiki/%E4%BC%BD%E8%97%8D%E3%81%A8%E3%83%90%E3%82%B6%E3%83%BC%E3%83%AB)』の中で、[リーナス・トーバルズ](https://ja.wikipedia.org/wiki/%E3%83%AA%E3%83%BC%E3%83%8A%E3%82%B9%E3%83%BB%E3%83%88%E3%83%BC%E3%83%90%E3%83%AB%E3%82%BA)に敬意を表して名付けられました。

### メトカーフの法則

[メトカーフの法則-Wikipedia](https://ja.wikipedia.org/wiki/%E3%83%A1%E3%83%88%E3%82%AB%E3%83%BC%E3%83%95%E3%81%AE%E6%B3%95%E5%89%87)

> ネットワーク理論では、システムの価値は、システムの利用者数の約2乗で成長します。

この法則は、システム内で可能なペアワイズ接続の数に基づいており、 [リードの法則](#リードの法則)と密接に関連しています。オドリズコらは、リードの法則とメトカーフの法則の両方が、ネットワーク効果に関する人間の認知の限界を考慮しないことによって、システムの価値を過大評価していると主張しています。 [ダンバー数を](#ダンバー数)参照してください。

関連項目:

- [リードの法則](#リードの法則)
- [ダンバー数](#ダンバー数)

### ムーアの法則

[ムーアの法則-Wikipedia](https://ja.wikipedia.org/wiki/%E3%83%A0%E3%83%BC%E3%82%A2%E3%81%AE%E6%B3%95%E5%89%87)

> 集積回路のトランジスタ数は約2年ごとに倍増します。

この法則は半導体やチップ技術の進歩の速さを示すためによく使われますが、ムーアの予測は1970年代から2000年代後半にかけて非常に正確であることが証明されています。近年では、その傾向はわずかに変化していますが、その理由の一部には[コンポーネントを小型化できる程度の物理的な制限(トンネル効果)](https://ja.wikipedia.org/wiki/%E3%83%88%E3%83%B3%E3%83%8D%E3%83%AB%E5%8A%B9%E6%9E%9C)があります。しかし、並列化の進歩や、半導体技術や量子コンピューティングにおける革命的な変化により、ムーアの法則が今後数十年にわたって真実であり続ける可能性があることを意味しています。

### マーフィーの法則/ソッドの法則

[マーフィーの法則-Wikipedia(](https://ja.wikipedia.org/wiki/%E3%83%9E%E3%83%BC%E3%83%95%E3%82%A3%E3%83%BC%E3%81%AE%E6%B3%95%E5%89%87)

> 何をやってもうまくいかないものはうまくいかない。

[エドワード・A・マーフィー・ジュニア](https://ja.wikipedia.org/wiki/%E3%82%A8%E3%83%89%E3%83%AF%E3%83%BC%E3%83%89%E3%83%BBA%E3%83%BB%E3%83%9E%E3%83%BC%E3%83%95%E3%82%A3%E3%83%BC%E3%83%BB%E3%82%B8%E3%83%A5%E3%83%8B%E3%82%A2)に関連して、*マーフィーの法則*では、物事がうまくいかないことがあれば、それはうまくいかないだろうということが述べられています。

これは開発者の間でよくある格言です。開発中、テスト中、あるいは本番中にも予期せぬことが起こることがあります。これは、 *ソッドの法則* （イギリス英語ではより一般的）にも関連しています。

> 何かがうまくいかないことがあれば、最悪のタイミングでそうなる。

これらの「法則」は、一般的にコミカルな意味で使われています。ただし、 [*確証バイアス*](#TODO)や[*選択バイアス*](#TODO)などの現象は、人々がこれらの法則を強調しすぎてしまう可能性があります(物事がうまくいく時の大半は、彼らは気づかれないですが、失敗は、しかし、より顕著であり、より多くの議論を生みます)。

関連項目:

- [確証バイアス](#TODO)
- [選択バイアス](#TODO)

### オッカムの剃刀

[オッカムの剃刀-Wikipedia](https://ja.wikipedia.org/wiki/%E3%82%AA%E3%83%83%E3%82%AB%E3%83%A0%E3%81%AE%E5%89%83%E5%88%80)

> エンティティは必要なくして掛け算してはいけない。
> オッカムのウィリアム

オッカムの剃刀は、いくつかの可能な解決策の中で、最も可能性の高い解決策は、概念と仮定の数が最も少ないものであると言います。この解は最も単純で、与えられた問題だけを解決し、偶発的な複雑さや起こりうる負の結果を導入することはありません。

関連項目:

- [YAGNI](#yagni)
- [銀の弾などない：偶発的な複雑さと本質的な複雑さ](https://ja.wikipedia.org/wiki/%E9%8A%80%E3%81%AE%E5%BC%BE%E3%81%AA%E3%81%A9%E3%81%AA%E3%81%84)

例:

- [リーンソフトウェア開発：無駄をなくす-Wikipedia(英語版)](https://en.wikipedia.org/wiki/Lean_software_development#Eliminate_waste)

### パーキンソンの法則

[パーキンソンの法則-Wikipedia](https://ja.wikipedia.org/wiki/%E3%83%91%E3%83%BC%E3%82%AD%E3%83%B3%E3%82%BD%E3%83%B3%E3%81%AE%E6%B3%95%E5%89%87)

> 仕事の量は、与えられた時間を全て満たすまで膨張する。

元の文脈では、この法則は官僚機構の研究に基づいていた。この法則は、ソフトウェア開発の取り組みに悲観的に適用されるかもしれません。理論的には、チームは締め切りが近づくまで非効率的であり、その後、締め切りまでに仕事を完成させようと急ぐので、実際の締め切りはやや恣意的になるということです。

この法則が[ホフスタッターの法則](#ホフスタッターの法則)と組み合わされた場合、さらに悲観的な見方が得られます。作業は、その完了に利用できる時間を埋めるために拡大し*、予想よりも長くかかり*ます。

関連項目:

- [ホフスタッターの法則](#ホフスタッターの法則)

### 早すぎる最適化

[最適化する時期-Wikipedia](https://ja.wikipedia.org/wiki/%E6%9C%80%E9%81%A9%E5%8C%96_(%E6%83%85%E5%A0%B1%E5%B7%A5%E5%AD%A6)#%E6%9C%80%E9%81%A9%E5%8C%96%E3%81%99%E3%82%8B%E6%99%82%E6%9C%9F)

> 早すぎる最適化は諸悪の根源です。
> [（ドナルドクヌース）](https://twitter.com/realdonaldknuth?lang=en)

Donald Knuthの論文「 [Structured Programming With Go To Statements」で](http://wiki.c2.com/?StructuredProgrammingWithGoToStatements) 、彼は次のように書いています。「プログラマーは、プログラムの重要でない部分の速度について考えたり、心配したりして膨大な量の時間を浪費している。小さな効率性、つまり97%程度の効率性については忘れた方がいいでしょう。 **早すぎる最適化は諸悪の根源です** 。しかし、その重要な3％で機会を逃してはなりません。」

しかし、 *早すぎる最適化*は（負荷の低い用語で）、必要性を知る前に最適化することと定義することができます。

### パットの法則

[パットの法則-Wikipedia(英語版)](https://en.wikipedia.org/wiki/Putt%27s_Law_and_the_Successful_Technocrat)

> 技術は、管理しないことを理解している人と、理解していないことを管理している人の2つのタイプに支配されている。

よくパットの法則にはパットの帰結が続きます。

> すべての技術的な階層は、時間の経過とともに、能力の逆転を発生させます。

これらの記述は、グループがどのように組織化されるかという様々な選択基準や傾向のために、技術的な組織の実務レベルには熟練した人が多く、管理職には自分が管理している仕事の複雑さや課題を認識していない人が多くいることを示唆しています。これは[、ピーター原理](#ピーターの原則)や[ディルバート原理](#ディルバートの原理)などの現象が原因である可能性があります。

ただし、このような法則は広範に一般化されており、*特定*の一部の組織には適用されますが、他の組織には適用されない場合があることを強調しておく必要があります。

関連項目:

- [ピーターの原則](#ピーターの原則)
- [ディルバートの原理](#ディルバートの原理)

### リードの法則

[リードの法則-Wikipedia(英語版)](https://en.wikipedia.org/wiki/Reed's_law)

> 大規模ネットワーク、特にソーシャルネットワークの効用は、ネットワークの大きさに応じて指数関数的にスケーリングする。

この法則はグラフ理論に基づいており、実用性は可能なサブグループの数に応じてスケールし、これは参加者の数や可能なペアワイズ接続の数よりも速くスケールします。オドリズコ氏らは、ネットワークの影響に対する人間の認識の限界を考慮しないことで、リードの法則がシステムの有用性を誇張していると主張しています。 [ダンバー数を](#ダンバー数)参照してください。

関連項目:

- [メトカーフの法則](#メトカーフの法則)
- [ダンバー数](#ダンバー数)

### 複雑性保存の法則（テスラーの法則）

[The Law of Conservation of Complexity-Wikipedia(英語版)](https://en.wikipedia.org/wiki/Law_of_conservation_of_complexity)

この法則では、システムには削減できない一定の複雑さがあるとされています。

システムの複雑さの中には、「不注意」なものもあります。これは、構造の不備、ミス、または解決すべき問題のモデリングの不備の結果です。不注意な複雑さは、減らすことができます（または排除することができます）。しかし、いくつかの複雑さは、解決される問題に内在する複雑さの結果として「内在的」です。この複雑さは動かすことはできますが、排除することはできません。

この法則の興味深い側面は、システム全体を単純化しても、本質的な複雑さは軽減されず、より複雑な方法でシステムを動かす*ユーザーに複雑性が移される*という提案です。

### 漏れのある抽象化の法則

[漏れのある抽象化の法則 Joel on Software(英語)](https://www.joelonsoftware.com/2002/11/11/the-law-of-leaky-abstractions/)

> 自明でない抽象化はすべて、程度の差こそあれ、漏れがある。
> （ [ジョエル・スポルスキー](https://twitter.com/spolsky) ）

この法則では、複雑なシステムでの作業を簡略化するためにコンピューティングで一般的に使用される抽象化は、特定の状況では、基礎となるシステムの要素を「漏らし」、抽象化が予期しない方法で動作することになると述べています。

例としては、ファイルをロードしてその内容を読むことが挙げられます。ファイルシステム API は低レベルのカーネルシステムの *抽象化*であり、それ自体が磁気プラッター (または SSD のフラッシュメモリ) 上のデータの変更に関連する物理的なプロセスを抽象化したものです。ほとんどの場合、ファイルをバイナリデータのストリームのように扱うという抽象化が機能します。磁気ドライブの場合、データを連続的に読み込むと、ランダム・アクセスよりも（ページ・フォルトのオーバーヘッドが増加するため）*大幅に*速くなりますが、SSD ドライブの場合は、このオーバーヘッドは存在しません。この場合に対処するためには、基本的な詳細を理解する必要があります（例えば、データベースのインデックスファイルはランダムアクセスのオーバーヘッドを減らすために構造化されています）が、抽象化された実装の詳細は、開発者が注意する必要があるかもしれません。

上記の例は、より多くの抽象化が導入されると、*より*複雑になる可能性があります。Linux オペレーティングシステムでは、ネットワーク経由でファイルにアクセスすることができますが、ローカルでは「通常の」ファイルとして表現されます。この抽象化は、ネットワーク障害が発生した場合に「漏れ」ます。開発者がこれらのファイルをネットワークの遅延や障害の影響を受ける可能性があることを考慮せずに「通常の」ファイルとして扱ってしまうと、解決策がバグだらけになってしまいます。

この法則を説明している記事によると、抽象化への過度の依存は、基礎となるプロセスの理解不足と相まって、実際には手元にある問題への対処を、場合によっては*より*複雑なものにしてしまうことが示唆されています。

関連項目:

- [ハイラムの法則](#ハイラムの法則暗黙のインターフェースの法則)

実際の例：

- [Photoshop Slow Startup](https://forums.adobe.com/thread/376152) - 過去に遭遇した問題 Photoshopの起動が遅く、数分かかることもありました。問題は、起動時に現在のデフォルトプリンタに関する情報を読み取ることだったようです。しかし、そのプリンタが実際にネットワークプリンタである場合、これは非常に長い時間がかかる可能性があります。ネットワークプリンタがローカルプリンタと同様に*抽象化*してしまったことにより接続時間の問題を引き起こしました。

### パーキンソンの凡俗法則

[パーキンソンの凡俗法則-Wikipedia](https://ja.wikipedia.org/wiki/%E3%83%91%E3%83%BC%E3%82%AD%E3%83%B3%E3%82%BD%E3%83%B3%E3%81%AE%E5%87%A1%E4%BF%97%E6%B3%95%E5%89%87)

この法則は、グループが深刻で実質的なものよりも、些細な問題や表面上の問題にはるかに多くの時間と注意力を注ぐことを示唆しています。

よくある架空の例は、原子力発電所の計画を承認する委員会の例であり、彼らは発電所自体のはるかに重要な設計よりも、自転車小屋の構造について議論することに時間の大半を費やしている。非常に大きく複雑なテーマについての議論では、高度な専門知識や準備がなければ、意味のあるな意見を述べることは難しいかもしれません。しかし、人々は意味のある意見を発言していると見られたいと思う傾向があり、そのため、簡単に推論できるが、必ずしも特別な重要性があるわけではないような些細なことに時間を集中させてしまう傾向がある。

上記の架空の例では、些細な細部に時間を浪費するための表現として「自転車シェディング」という用語を使用しました。関連用語は「 [ヤクシェービング](https://ja.wiktionary.org/wiki/yak_shaving) 」です。これは、メインタスクの前提条件の長い連鎖の一部である、一見無関係な活動を意味します。

### UNIX哲学

[UNIX哲学-Wikipedia](https://ja.wikipedia.org/wiki/UNIX%E5%93%B2%E5%AD%A6)

UNIX理念は、ソフトウェアの構成要素は小さく、一つの特定のことをうまく行うことに集中すべきであるというものです。これは、大規模で複雑な多目的プログラムを使うのではなく、小さくてシンプルで、よく定義されたユニットを組み合わせてシステムを構築することを容易にすることができます。

現代における「マイクロサービス・アーキテクチャ」は、この法則の応用と考えることができ、サービスは小さく、焦点を絞って、特定の一つのことをしっかりと行うことで、複雑な動作をシンプルなビルディングブロックで構成することを可能にしています。

### Spotifyモデル

[Spotifyモデル-Spotify Labs(英語)](https://labs.spotify.com/2014/03/27/spotify-engineering-culture-part-1/)

Spotifyモデルとは、「Spotify」によって普及したチームと組織構造へのアプローチです。このモデルでは、チームはテクノロジーではなく機能を中心に組織されています。

また、Spotify モデルでは、組織構造の他の要素である部族、ギルド、チャプターの概念も普及しています。

### ワドラーの法則

[ワドラーの法則-wiki.haskell.org(英語)](https://wiki.haskell.org/Wadler's_Law)

> どのような言語設計においても、このリストの特徴を議論するのに費やされた時間の合計は、その位置の累乗に2を上げることに比例します。
> 1. 意味論
> 2. 構文
> 3. 字句構文
> 4. コメントの字句構文
> （要するに、意味論に1時間使うとすると、8時間はコメントの構文に費やされます）。

同様に[パーキンソンの凡俗法則](#パーキンソンの凡俗法則) 、和ドラーの法則は、言語を設計する際に、言語構造の重要性に比べて、言語構造に費やされる時間が不釣り合いに多いということが述べられています。

関連項目:

- [パーキンソンの凡俗法則](#パーキンソンの凡俗法則)

### ウィートンの法則

[リンク(英語)](http://www.wheatonslaw.com/)

[公式日(英語)](https://dontbeadickday.com/)

> 嫌な奴になるな
> *ウィル・ウィートン*

ウィル・ウィートン（スタートレック：ネクスト・ジェネレーション、ビッグバン・セオリー）によって考案されたこのシンプルで簡潔で強力な法則は、専門的な組織内での調和と尊敬を高めることを目的としています。同僚との会話、コードレビューの実行、他の視点からの反論、批評、そして一般的に、ほとんどのプロフェッショナルな人間関係に適用することができます。

## 原則

一般に、原則は設計に関するガイドラインである可能性が高くなります。

### ディルバートの原理

[ディルバートの法則-Wikipedia](https://ja.wikipedia.org/wiki/%E3%83%87%E3%82%A3%E3%83%AB%E3%83%90%E3%83%BC%E3%83%88%E3%81%AE%E6%B3%95%E5%89%87)

> 企業は、事業への損害を最小限にとどめるために、系統立てて無能な者から管理職に昇進させて行く傾向がある
> *スコットアダムス*

スコット・アダムス（漫画「ディルバート」の作者）が開発した経営概念で、ディルバート原則は[、ピーター原則に](#ピーターの原則)触発されています。ディルバートの原則では、有能でない社員を管理職に昇格させることで、事業への損害を最小限にとどめる。 Adamsは、1995年のウォールストリートジャーナルの記事でこの原則を最初に説明し、1996年のビジネスブック、 [The Dilbert Principleで](#関連書籍)それを拡張しました。

関連項目:

- [ピーターの原則](#ピーターの原則)
- [パットの法則](#パットの法則)

### パレート原理（80/20ルール）

[パレートの法則-Wikipedia](https://ja.wikipedia.org/wiki/%E3%83%91%E3%83%AC%E3%83%BC%E3%83%88%E3%81%AE%E6%B3%95%E5%89%87)

> 人生のほとんどのものが均等に分配されていません。

パレートの原理は、いくつかのケースでは、結果の大部分は少数の入力から来ることを示唆している。

- 特定のソフトウェアの80％は、割り当てられた合計時間の20％で実装できます（逆に、コードの最も難しい20％部分を実装するのに時80％の時間がかかります）
- 2割の努力は8割の結果を生む
- 2割の仕事が8割の収益を生み出す
- 20%のバグが80%のクラッシュを引き起こす
- 20%の機能が80%の使用率を引き起こす

 1940年代には、品質管理の父と広く信じられているアメリカ・ルーマニアのエンジニア、ジョセフ・ジュラン博士が[、パレートの原則を品質問題に適用し始めました](https://en.wikipedia.org/wiki/Joseph_M._Juran) 。

この原則は、次のようにも知られています。80/20ルール、バイタル・フューの法則、ファクター・スパーシティの原理。

実際の例：

- 2002年に、Microsoftは、最も報告されたバグの上位20％を修正することにより、windowsやofficeの関連するエラーやクラッシュの80%が解消されると報告しています（ [参考文献](https://www.crn.com/news/security/18821726/microsofts-ceo-80-20-rule-applies-to-bugs-not-just-features.htm) ）。

### ピーターの原則

[ピーターの法則-Wikipedia](https://ja.wikipedia.org/wiki/%E3%83%94%E3%83%BC%E3%82%BF%E3%83%BC%E3%81%AE%E6%B3%95%E5%89%87)

> 階層社会では、人間は能力の極限まで出世する。
> *ローレンス・J・ピーター*

ローレンス・J・ピーターによって開発された経営概念で、ピーターの原則は、仕事が得意な人は、もはや成功しないレベル（彼らの「無能のレベル」）に達するまで、昇進すると観察しています。この時点では、彼らはより熟練であるため、組織から外される可能性は低く、彼らを成功に導いた元々のスキルが必ずしも新しい仕事に必要なスキルであるとは限らないため、彼らが本来持っているスキルがほとんどない役割に留まり続けることになります。

これは、最初はエンジニアとしてキャリアをスタートさせ、他のエンジニアの*管理に*つながるキャリアパスを描いているエンジニアにとって、特に興味深いものです。管理職には、根本的にエンジニアとは異なるスキルセットが必要です。

関連項目:

- [ディルバートの原理](#ディルバートの原理)
- [パットの法則](#パットの法則)

### 堅牢性の原則（ポステルの法則）

[堅牢性の原則-Wikipedia(英語版)](https://en.wikipedia.org/wiki/Robustness_principle)

> 自分のやることは慎重に、他人から受け入れるときは自由に。

サーバーアプリケーションの開発によく適用されるこの原則は、他のシステムに送るものは可能な限り最小限にして、適合性のあるものにすべきであるが、処理できる場合には、適合性のない入力を許容することを目指すべきである、ということを述べています。

この原則の目標は、ハンドルできる場合には、不適合な入力を処理できるので、堅牢なシステムを構築することです。しかし、特にそのような入力の処理が十分にテストされていない場合には、不適合な入力を受け入れることにはセキュリティ上の問題がある可能性があります。

不適合な入力を許可すると、実装者が最終的にこの自由に依存して機能を構築するようになるため、プロトコルが進化する可能性が損なわれる場合があります。

関連項目:

- [ハイラムの法則](#ハイラムの法則暗黙のインターフェースの法則)

### SOLID

これは以下を指す頭字語です。

- S： [単一責任の原則](#単一責任の原則)
- O： [開放/閉鎖原則](#開放閉鎖原則)
- L： [リスコフ代替原則](#リスコフの置換原則)
- I： [インターフェース分離の原則](#インターフェース分離の原則)
- D： [依存関係の逆転の原則](#依存性逆転の原則)

これらは、 [オブジェクト指向プログラミングの](#todo)主要な原則です。このような設計原則は、開発者が保守しやすいシステムを構築するのに役立つはずです。

### 単一責任の原則

[単一責任原則-Wikipedia(英語版)](https://en.wikipedia.org/wiki/Single_responsibility_principle)

> すべてのモジュールやクラスは、単一の責任のみを持つべきです。

「 [SOLID](#solid) 」第一原則。この原則は、モジュールやクラスは一つのことを一つのことだけを行うべきだということを提案しています。より実用的な用語では、これはプログラムの機能への単一の小さな変更は、1つのコンポーネントのみの変更を必要とすることを意味します。例えば、パスワードの複雑さを検証する方法を変更するには、プログラムの一部分だけを変更する必要があります。

理論的には、これによりコードがより堅牢になり、変更が容易になるはずです。変更されるコンポーネントが単一の責任を持っていることを知ることは、その変更の*テスト*がより簡単になることを意味します。先ほどの例を使うと、パスワードの複雑さのコンポーネントを変更することは、パスワードの複雑さに関連する機能にのみ影響を与えることができるはずです。多くの責任を持つコンポーネントへの変更の影響を推論することは、はるかに難しいでしょう。

関連項目:

- [オブジェクト指向プログラミング](#todo)
- [SOLID](#solid)

### 開放/閉鎖原則

[開放/閉鎖原則-Wikipedia](https://ja.wikipedia.org/wiki/%E9%96%8B%E6%94%BE/%E9%96%89%E9%8E%96%E5%8E%9F%E5%89%87)

> エンティティは拡張のために開かれ、修正のために閉じられるべきです。

「 [SOLID](#solid) 」第二原則。この原則では、エンティティー（クラス、モジュール、関数など）は動作を*拡張*することができなければならないが、 *既存*の振る舞いは修正することができないべきではないということを述べています。

仮定としてMarkdown文書をHTMLに変換することができるモジュールを想像してください。モジュールがモジュール内部を修正することなく、新しく提案されたMarkdown機能を処理するために拡張できた場合、拡張のためにオープンになります。既存のMarkdown機能が処理されるように、モジュールが利用者によって*修正されない*場合、修正のために*クローズド*になります。

この原則は、オブジェクト指向プログラミングに特に関連しています。簡単に拡張するオブジェクトを設計するかもしれませんが、予期しない方法で変更された既存の動作を持つことができるオブジェクトを設計することを避けます。

関連項目:

- [オブジェクト指向プログラミング](#todo)
- [SOLID](#solid)

### リスコフの置換原則

[リスコフの置換原則-Wikipedia](https://ja.wikipedia.org/wiki/%E3%83%AA%E3%82%B9%E3%82%B3%E3%83%95%E3%81%AE%E7%BD%AE%E6%8F%9B%E5%8E%9F%E5%89%87)

> システムを壊すことなく、タイプをサブタイプに置き換えることができるはずです。

「 [SOLID](#solid) 」原則の3番目。この原則は、コンポーネントがタイプに依存している場合、システムに障害が発生したり、そのサブタイプが何であるかの詳細を知る必要なく、そのタイプのサブタイプを使用できるはずであると述べています。

例として、ファイルを表す構造からXMLドキュメントを読み取るメソッドがあるとします。メソッドが基本タイプ「ファイル」を使用する場合、「ファイル」から派生するものはすべて関数で使用できるはずです。 「ファイル」が逆方向のシークをサポートし、XMLパーサーがその関数を使用するが、逆型シークが試行されたときに派生型「ネットワークファイル」が失敗する場合、「ネットワークファイル」は原則に違反しています。

この原則は、オブジェクト指向プログラミングに特に関連しています。システムのユーザーを混乱させないように、型階層を注意深くモデル化する必要があります。

関連項目:

- [オブジェクト指向プログラミング](#todo)
- [SOLID](#solid)

### インターフェース分離の原則

[インターフェース分離原則-Wikipedia(英語版)](https://en.wikipedia.org/wiki/Interface_segregation_principle)

> 使用しないメソッドに依存することを強制されるクライアントはありません。

「 [SOLID](#solid) 」原則の4番目。この原則は、コンポーネントのコンシューマーが、実際に使用しないコンポーネントの機能に依存すべきではないと述べています。

例として、ファイルを表す構造体からXML文書を読み込むメソッドがあるとします。このメソッドが必要とするのは、ファイル内のバイトを読み込んだり、前に移動したり、後ろに移動したりすることだけです。ファイル構造体の無関係な機能が変更されたためにこのメソッドを更新する必要がある場合（ファイルのセキュリティを表現するために使用されるパーミッションモデルの更新など）、その原則は無効になっています。ファイルは「シーク可能なストリーム」インターフェースを実装し、XMLリーダーはそれを使用する方が良いでしょう

この原則はオブジェクト指向プログラミングに特に関連性があり、インターフェイス、階層構造、抽象型が異なるコンポーネント間の結合を[最小限](#todo)にするために使用されます。[ダックタイピング](#todo)は、明示的なインターフェースを排除することでこの原則を強制する方法論です。

関連項目:

- [オブジェクト指向プログラミング](#todo)
- [SOLID](#solid)
- [ダックタイピング](#todo)
- [デカップリング](#todo)

### 依存性逆転の原則

[依存性逆転の原則-Wikipedia](https://ja.wikipedia.org/wiki/%E4%BE%9D%E5%AD%98%E6%80%A7%E9%80%86%E8%BB%A2%E3%81%AE%E5%8E%9F%E5%89%87)

> 高レベルのモジュールは、低レベルの実装に依存すべきではありません。

「 [SOLID](#solid) 」原則の5番目。この原則は、より高いレベルのオーケストレーションコンポーネントは、依存関係の詳細を知っている必要はないことを述べています。

例として、ウェブサイトからメタデータを読み取るプログラムがあるとします。メインコンポーネントは、ウェブページのコンテンツをダウンロードするためのコンポーネントについて知る必要があり、メタデータを読み取ることができるコンポーネントであると想定します。依存関係の逆転を考慮すると、メインコンポーネントは、バイトデータをフェッチできる抽象コンポーネントと、バイトストリームからメタデータを読み取ることができる抽象コンポーネントのみに依存します。メインコンポーネントは、TCP / IP、HTTP、HTMLなどについては認識しません。

この原則は複雑です。システムの予想される依存関係（したがって、名前）を「逆転」するように見える場合があるためです。実際には、別のオーケストレーションコンポーネントが抽象型の正しい実装が使用されていることを確認する必要があることも意味します（たとえば、前の例では、 *何か*がメタデータリーダーコンポーネントにHTTPファイルダウンローダーとHTMLメタタグリーダーを提供する必要があります）。次に、 [Inversion of Control](#todo)や[Dependency Injection](#todo)などのパターンに触れます。

関連項目:

- [オブジェクト指向プログラミング](#todo)
- [SOLID](#solid)
- [制御の反転](#todo)
- [依存性注入](#todo)

### DRY原則

[Don't repeat yourself-Wikipedia](https://ja.wikipedia.org/wiki/Don%27t_repeat_yourself)

> すべての知識は、システム内で単一の明確で信頼できる表現を持つ必要があります。

DRYは、 *Do n't Repeat Yourselfの*頭字語です。この原則は、開発者がコードの繰り返しを減らして情報を1か所に保管できるようにすることを目的としており、1999年にAndrew HuntとDave Thomasが 『 [The Pragmatic Developer](https://en.wikipedia.org/wiki/The_Pragmatic_Programmer) 』で引用しています。

> DRYの反対は*WET* （すべてを2回書き込むか、タイピングを楽しむ）です。

実際には、2つ（またはそれ以上）の異なる場所に同じ情報がある場合、DRYを使用してそれらを1つの場所にマージし、必要な場所で必要に応じて再利用できます。

関連項目

- [実用的な開発者(英語)](https://en.wikipedia.org/wiki/The_Pragmatic_Programmer)

### KISSの原則

[KISSの原則-Wikipedia](https://ja.wikipedia.org/wiki/KISS%E3%81%AE%E5%8E%9F%E5%89%87)

> 簡潔に単純にしておけ

KISSの原則は、ほとんどのシステムは複雑にするのではなく、シンプルに保つことが最もよく機能するというもので、シンプルさは設計の重要な目標であり、不必要な複雑さは避けるべきだというものです。 1960年にアメリカ海軍で始まったこのフレーズは、航空機エンジニアのケリー・ジョンソンに関連しています。

この原則は、ジョンソンが設計エンジニアのチームに一握りの工具を渡し、設計しているジェット機は、現場の平均的な整備士がこれらの工具だけで戦闘状況下で修理可能なものでなければならないという課題を与えたという話に最もよく例示されています。したがって、「バカ」とは、技術者自身の能力ではなく、物の壊れ方と、それを修理するために利用できる道具の巧妙さの関係を指しています。

関連項目:

- [ゴールの法則](#ゴールの法則)

### YAGNI

[YAGNI-Wikipedia](https://ja.wikipedia.org/wiki/YAGNI)

 ***Y**ou **A**in't **G**onna **N**eed **I**t*"縮めて YAGNI

> 実際にそれらが必要なときに常に実装し、必要があると予測しただけでは決して実装しないでください。
> （ [Ron Jeffries](https://twitter.com/RonJeffries) ）（XPの共同創設者であり、「Extreme Programming Installed」という本の著者）

この*エクストリームプログラミング* （XP）の原則は、開発者は当面の要件に必要な機能のみを実装し、後で必要になる可能性のある機能を実装して将来を予測しようとする試みを避けることを示唆しています。

この原則を順守することで、コードベース内の未使用のコードの量を減らし、価値のない機能に時間と労力が浪費されるのを防ぐことができます。

関連項目

- [関連書籍：インストールされているExtremeプログラミング](#関連書籍)

### 分散コンピューティングの落とし穴

[分散コンピューティングの落とし穴-Wikipedia](https://ja.wikipedia.org/wiki/%E5%88%86%E6%95%A3%E3%82%B3%E3%83%B3%E3%83%94%E3%83%A5%E3%83%BC%E3%83%86%E3%82%A3%E3%83%B3%E3%82%B0%E3%81%AE%E8%90%BD%E3%81%A8%E3%81%97%E7%A9%B4)

「*ネットワークコンピューティングの落とし穴*」としても知られているこの落とし穴は、ソフトウェア開発の失敗につながる可能性のある、分散コンピューティングに関する思い込み(または信念)のリストです。仮定は以下の通りです。

- ネットワークは信頼できる
- 待ち時間はゼロです
- 帯域幅は無限です
- ネットワークは安全です
- トポロジーは変わらない
- 管理者が一人だけいます
- トランスポートコストはゼロ
- ネットワークは均一です

最初の4つの項目は、1991年頃に[Bill Joy](https://en.wikipedia.org/wiki/Bill_Joy)と[Tom Lyon](https://twitter.com/aka_pugs)によってリストされ、 [James Gosling](https://en.wikipedia.org/wiki/James_Gosling)によって最初に「ネットワークコンピューティングの失墜」として分類されました。 [L.ピータードイチュ](https://en.wikipedia.org/wiki/L._Peter_Deutsch)は、5、6、7番目の誤りを追加しました。 90年代後半、ゴスリングは8番目の誤りを追加しました。

このグループは、 [Sun Microsystemsの](https://en.wikipedia.org/wiki/Sun_Microsystems)内部で当時何が起こっていたかに触発されました。

これらの誤りは、弾力性のあるコードを設計するときに注意深く検討する必要があります。これらの誤りのいずれかが、分散システムの現実と複雑さに対処できない欠陥のあるロジックにつながる可能性があると仮定します。

関連項目:

- [分散コンピューティングの落とし穴の採餌（パート1）-Vaidehi Joshi
    中(英語)](https://medium.com/baseds/foraging-for-the-fallacies-of-distributed-computing-part-1-1b35c3b85b53)
- [Deutsch's Fallacies、10年後(英語)](http://java.sys-con.com/node/38665)

## 関連書籍:

もっと興味を感じたなら、以下の本を参照してください。

- [インストールされているエクストリームプログラミング-ロンジェフリーズ、アンアンダーソン、チェットヘンドリクソン](https://www.goodreads.com/en/book/show/67834) -エクストリームプログラミングのコア原則をカバーしています。
- [The Mythical Man Month-フレデリックP.ブルックスJr.-](https://www.goodreads.com/book/show/13629.The_Mythical_Man_Month)ソフトウェアエンジニアリングに関する古典的な巻。 [ブルックスの法則](#ブルックスの法則)は本の中心的なテーマです。
- [ゲーデル、エッシャー、バッハ：永遠のゴールデンブレイド-ダグラスR.ホフスタッター。](https://www.goodreads.com/book/show/24113.G_del_Escher_Bach) -この本は分類するのが難しいです。 [ホフスタッターの法則](#ホフスタッターの法則)は本からです。
- [ディルバートの原則-スコットアダムス](https://www.goodreads.com/book/show/85574.The_Dilbert_Principle) - [ディルバートの原則](#ディルバートの原理)を作成した作者によるアメリカの企業の漫画の外観。
- [ピーター原則-ローレンスJ.ピーター](https://www.goodreads.com/book/show/890728.The_Peter_Principle) - [ピーター原則の](#ピーターの原則)出典である、より大きな組織と人々の管理の課題に関する別の漫画の見方。

## 翻訳

多くの素晴らしい投稿者のおかげで、ハッカーの法則は多くの言語で利用可能です。モデレーターのスポンサーもご検討ください。

言語 | モデレータ | ステータス
--- | --- | ---
[🇧🇷 Brasileiro / Brazilian](../translations/pt-BR.md) | [Eugênio Moreira](https://github.com/eugenioamn), [Leonardo Costa](https://github.com/leofc97) | [![gitlocalized ](https://gitlocalize.com/repo/2513/pt-BR/badge.svg)](https://gitlocalize.com/repo/2513/pt-BR?utm_source=badge)[](https://gitlocalize.com/repo/2513/pt-BR?utm_source=badge)[](https://gitlocalize.com/repo/2513/pt-BR?utm_source=badge)
[🇨🇳 中文 / Chinese](https://github.com/nusr/hacker-laws-zh) | [Steve Xu](https://github.com/nusr) | Partially complete
[🇩🇪 Deutsch / German](../translations/de.md) | [Vikto](https://github.com/viktodergunov) | [![gitlocalized ](https://gitlocalize.com/repo/2513/de/badge.svg)](https://gitlocalize.com/repo/2513/de?utm_source=badge)[](https://gitlocalize.com/repo/2513/de?utm_source=badge)[](https://gitlocalize.com/repo/2513/de?utm_source=badge)
[🇫🇷 Français / French](../translations/fr.md) | [Kevin Bockelandt](https://github.com/KevinBockelandt) | [![gitlocalized ](https://gitlocalize.com/repo/2513/fr/badge.svg)](https://gitlocalize.com/repo/2513/fr?utm_source=badge)[](https://gitlocalize.com/repo/2513/fr?utm_source=badge)[](https://gitlocalize.com/repo/2513/fr?utm_source=badge)
[🇬🇷 ελληνικά / Greek](../translations/el.md) | [Panagiotis Gourgaris](https://github.com/0gap) | [![gitlocalized ](https://gitlocalize.com/repo/2513/el/badge.svg)](https://gitlocalize.com/repo/2513/el?utm_source=badge)[](https://gitlocalize.com/repo/2513/el?utm_source=badge)[](https://gitlocalize.com/repo/2513/el?utm_source=badge)
[🇮🇹 Italiano / Italian](https://github.com/csparpa/hacker-laws-it) | [Claudio Sparpaglione](https://github.com/csparpa) | Partially complete
[🇰🇷 한국어 / Korean](https://github.com/codeanddonuts/hacker-laws-kr) | [Doughnut](https://github.com/codeanddonuts) | Partially complete
[🇱🇻 Latviešu Valoda / Latvian](../translations/lv.md) | [Arturs Jansons](https://github.com/iegik) | [![gitlocalized ](https://gitlocalize.com/repo/2513/lv/badge.svg)](https://gitlocalize.com/repo/2513/lv?utm_source=badge)[](https://gitlocalize.com/repo/2513/lv?utm_source=badge)[](https://gitlocalize.com/repo/2513/lv?utm_source=badge)
[🇷🇺 Русская версия / Russian](https://github.com/solarrust/hacker-laws) | [Alena Batitskaya](https://github.com/solarrust) | Partially complete
[🇪🇸 Castellano / Spanish](../translations/es-ES.md) | [Manuel Rubio](https://github.com/manuel-rubio) ([Sponsor](https://github.com/sponsors/manuel-rubio)) | Partially complete
[🇹🇷 Türkçe / Turkish](https://github.com/umutphp/hacker-laws-tr) | [Umut Işık](https://github.com/umutphp) | [![gitlocalized ](https://gitlocalize.com/repo/2513/tr/badge.svg)](https://gitlocalize.com/repo/2513/tr?utm_source=badge)[](https://gitlocalize.com/repo/2513/tr?utm_source=badge)[](https://gitlocalize.com/repo/2513/tr?utm_source=badge)
| [JP 日本語 / Japanese](../translations/jp.md) | [Fumikazu Fujiwara](https://github.com/freddiefujiwara)|Partially complete  |

翻訳を更新したい場合は、 [open a pull request](https://github.com/dwmkerr/hacker-laws/pulls)するだけです。新しい言語を追加したい場合は、 [GitLocalize](https://gitlocalize.com/) にログインしてアカウントを作成し、言語の管理を依頼するためのissueを開いてください。また、上の表とファイルの先頭にあるリンクを更新するプルリクエストを開いていただけると、とても助かります。

## 関連プロジェクト

- [今日のヒント(英語)](https://tips.darekkay.com/html/hacker-laws-en.html) -毎日ハッカーの法則/原則の更新を知ることができます。
- [ハッカーの法則コマンド](https://github.com/umutphp/hacker-laws-cli)あなたの端末上でランダムな法則を一覧表示、表示、確認できます。

## 貢献方法

貢献してください! 追加や変更を提案したい場合は  [Raise an issue](https://github.com/dwmkerr/hacker-laws/issues/new)、変更を提案したい場合は  [Open a pull request](https://github.com/dwmkerr/hacker-laws/compare) をご利用ください。

文章やスタイルなどの要件については、[Contributing Guidelines](./.github/contributing.md)  を必ずお読みください。プロジェクトの議論に参加する際には、[Code of Conduct](./.github/CODE_OF_CONDUCT.md)を意識してください。

## TODO

こんにちは！あなたがここに来たということは、私がまだ書き上げていないトピックへのリンクをクリックしたことにですね。

リクエストしたい場合は  [Raise an Issue](https://github.com/dwmkerr/hacker-laws/issues) をクリックするか、トピックの定義案を提出したい場合は [Open a Pull Request](https://github.com/dwmkerr/hacker-laws/pulls) をクリックしてください。
