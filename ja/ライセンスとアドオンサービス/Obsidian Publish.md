Obsidian Publish™ はノートをホスティングして公開する有料のサービスです。

Obsidianのアプリケーション内からノートを公開する方法についての説明は[[パブリッシュ|パブリッシュプラグイン]]を参照してください。

### プライバシー

[[パブリッシュ|パブリッシュプラグイン]]を介して公開するものについては保管庫全体を公開するか、保管庫内の選択したノートのみを公開するか、ユーザーによって完全にコントロールされます。**公開しないように**選択したすべてのノートについて、それらのノートは完全にプライベートであり、Obsidian Publishはその内容についてまったく感知しないことに確信を持つことができます。

### バックアップ

Obsidian Publishは内容のバックアップとしては利用することができないことに注意してください。また、どのようなバックアップの方法でもいいので、作成したサイトのバックアップコピーを常に自分自身で作成しておくようにしてください。Obsidian Publishはこれから、機能性と使いやすさ、そしてサイトの可用性によりフォーカスして開発していきます。

### デモンストレーション

公式サイトはObsidian Publishによって提供されており、公式サイトで既にこの記事を閲覧している場合にはよいデモンストレーションのチャンスとなります。

まだ見ていない場合には、こちらをご覧ください: https://publish.obsidian.md/help.

### 何が含まれますか

Obsidian Publishサービスでは公開したいノートを選択して、Obsidianのアプリケーション内から直接サイトを作成することが可能です。

サイトをカスタマイズしたい場合には、ライトモードとダークモードを選択できます。さらに読み取り可能な行長さを制限するかとフルページの長さに設定するかを切り替えることも可能です。

[[パブリッシュ|パブリッシュプラグイン]]から、有効･無効にできるいくつかの要素があります。これらのオプションの変更は、キャッシュがクリアされたら直ちにサイトに反映されます。通常は5分以内にキャッシュがクリアされます。

##### ナビゲーション

このオプションを有効にすると、ナビゲーションサイドバーにサイト内のすべての公開ページとフォルダが表示されるようになります。閲覧者が現在開いているノートがハイライトされて、クリックで他のノートへ移動することができます。

##### グラフビュー

現在開いているページのローカルグラフを表示します。これはObsidianの[[グラフビュー]]プラグインと同じレンダリングエンジンを使用しています。

##### 目次

現在開いているページの目次を表示します。[[アウトライン]]プラグインと同様にページ内の見出しからリストが生成されます。ノートを移動している閲覧者は、スクロールにあわせてハイライトされる見出しを見ることができ、見出しをクリックして直ちにそこへ移動することができます。

##### ホバープレビュー

サイト内のリンクにカーソルをあわせると、ポップアップボックス内で内容が表示されます。これはObsidianの[[ページプレビュー]]プラグインと同様に機能します。

##### バックリンク

各ページの最後に他のページからのバックリンクを含む｢Linked to this page｣のセクションを表示します。バックリンクが無い場合には、このセクションは表示されません。

##### カスタムCSS

サイトのスタイルをカスタマイズするには、`obsidian.css` か `publish.css` のどちらかをアップロードしてください。これらのファイルはサイトのルートフォルダに保存される必要があります。両方をアップロードすることもでき、既存の`obsidian.css` を利用して `publish.css` 内にてPublish用にいくつかの追加の調整を加えることができます。

##### ファビコン

サイトのファビコンを変更するには、任意のサイズの `png` 形式のアイコンを `favicon-32.png` または `favicon-32x32.png` の形式でアップロードできます。`favicon.ico` ファイルをアップロードすることもできます。これらのファイルはどのフォルダにも保存できます。現在の推奨サイズ(2020年現在において)は、`32×32`, `128x128`, `152×152`, `167x167`, `180x180`, `192x192` または `196x196` です。

### Coming up

Obsidian Publishはまだ開発の初期段階にあります。現在私たちはこれらの機能を追加する予定にあります。

- カスタムドメインのサポート
- 検索
- タグペインセクション
- より多くのビルトインテーマ

Obsidian Publishについての機能リクエストがある場合には[ここからフォーラムリクエスト](https://forum.obsidian.md/)を送信して私たちに知らせてください。

### 料金設定

Obsidian Publishの料金設定のついては、 [料金設定ページ](https://obsidian.md/pricing)をご覧ください。

### 技術的詳細

Obsidian Publishは世界中からの高速なアクセスを実現してサイトを配信するためにCloudflareをCDN(content delivery network)として使用しており、ユーザーサイトのコピーを200以上のデータセンターにおいてキャッシュするようにしています。これによって、たとえサイト閲覧者が私たちのプライマリサーバーから遠く離れたところに住んでいたとしても、待ち時間を少なくし、サイトは早いままで、高速にロードができるようしています。

しかしながら、上記のことはサイトの設定変更やコンテンツの新規公開や非公開などを行った際に、閲覧者がしばらくの間サイトの最新版を見ることができないということを意味しません。現在、私たちのキャッシュは、内容が変更されていないことを確認するため、｢再有効｣が必要になる前の一時間の間は保持されるよう構成されています。

公開した直後のアイテムについて、依然として古いバージョンのものが見える場合には、通常はリロードボタンを押してハードリフレッシュを実行し、ドロップダウンメニューからハードリロードを選択してください。うまくいかない場合は、利用しているブラウザのキャッシュを削除してみるか、ネットワークタブのデベロッパーツールを利用してキャッシュを無効化してみてください。

---

### 関連

ノートを公開するための詳細については[[パブリッシュ|パブリッシュプラグイン]]を参照してください。