## ソフトウェア開発共通ガイドライン

### ソフトウェア開発共通ガイドラインについて

- 本ガイドラインは、ソフトウェア開発における品質を担保するための共通したガイドラインになります
- アプリやファームといった分野や開発言語によらない一般的に遵守すべきルールについて定めています
- ガイドラインには項目ごとに以下のようなタグがついており、タグによってどの程度ガイドラインを遵守すべきかが変わります

| タグ                            | 遵守の必要性 |
| ----------------------------- | ------ |
| MUST / MUST NOT               | 必須     |
| RECOMMENDED / NOT RECOMMENDED | 推奨     |

### コミュニケーションガイドライン

#### 会議

- 【MUST】会議の目的を明確にしてください
- 【RECOMMENDED】アジェンダを事前に共有してください
- 【RECOMMENDED】議事録を作成し、決定事項や次のアクションを明確にしてください
- 【MUST】不要な会議は設定せず、必要な人だけが参加してください
- 【MUST】立場によらず、平等に発言できる場を心がけてください

#### 質問

- 【MUST】質問をする前に、必ず自己解決を試みてください（ドキュメントの確認や検索など）
- 【MUST】具体的かつ明確な質問を心がけてください
- 【RECOMMENDED】質問の背景（なぜこの質問をしたのか）や自分の考えもあわせて共有してください
- 【RECOMMENDED】自分が理解できたか、質問者に対して理解した内容を相手に伝えてください（正しく理解できたかの確認）

#### [参考]
- [質問は恥ではないし役に立つ](https://qiita.com/seki_uk/items/4001423b3cd3db0dada7)

#### チャット

- 【MUST】コミュニケーションツールを利用したオープンな場でのやり取りをこころがけてください
- 【NOT RECOMMENDED】各人が個別に口頭でのやりとりをおこなったり、閉じた場でのチャットをなるべく行わないようにしてください
- 【MUST】皆がオープンな場でのコミュニケーションが行えるような環境づくりに努めてください
- 【MUST】チャットする際は緊急度や重要度を明確にし、必要な人に対して適切にメンションを行うようにしてください
- 【RECOMMENDED】絵文字やリアクションを活用し、コミュニケーションを円滑にしてください

#### 振り返り

- 【MUST】チームや個人としての定期的な振り返りを行ってください
- 【RECOMMENDED】チームとしての改善事項は会議などで共有できる場を設定してください（プロジェクト管理者に対して）
- 【RECOMMENDED】個人としての振り返り・相談事項は1on1などで個別に相談できる場を設定してください（プロジェクト管理者に対して）

#### [参考]
- [KPTとは？](https://meetsmore.com/product-services/talent-management/media/93642)

### ソフトウェア品質ガイドライン

#### ドキュメント

- 【MUST】基本設計は必ず設計書としてドキュメントに記載してください
- 【MUST】ドキュメントは常に最新の状態を保ち、実装との整合性を保ってください
- 【MUST】設計書や仕様書は一元管理を行い、チーム全員がアクセス可能な場所で管理してください

#### レビュー

- 【MUST】成果物については、必ず1人以上のレビューを実施してください
- 【RECOMMENDED】レビュアーは複数人設定できる場合は、複数人設定してください
- 【MUST】建設的なフィードバックを心がけ、良い点も指摘してください
- 【RECOMMENDED】レビューコメントには、根拠や改善案を提示してください
- 【RECOMMENDED】予めどのような観点でレビューを行うのか、チェックシートを作成してください

#### [参考]
- [コードレビューのラベル](https://zenn.dev/hacobell_dev/articles/code-review-comment-prefix)

#### コーディングスタイル

- 【MUST】コーディングは、各プログラミング言語で一般的に使用されているスタイルを適用してください
- 【RECOMMENDED】関数名やメソッド名はわかりやすい名前をつけてください
- 【RECOMMENDED】関数やメソッドは単一責任の原則に従い、適切な長さに保つようにしてください

#### フォーマット・静的解析

- 【MUST】各言語に適したコードフォーマッターを使用し、一貫性を保つようにしてください
- 【MUST】各言語に適した静的解析を導入し、潜在的な問題を解決するようにしてください
- 【RECOMMENDED】GitHub ActionsなどCI/CDツールを組み込み、自動でフォーマッターや静的解析のチェックを行うようにしてください