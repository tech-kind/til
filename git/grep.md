## 文字列検索

- 全部のブランチから文字列を検索する方法

1. リモートにあるものを取りこぼさないように、`git fetch`をしておく

``` sh
$ git fetch
```

2. 以下のコマンドで特定のキーワードを抽出する

``` sh
$ git grep 【キーワード】 $(git branch -a --format='%(objectname) %(refname:short)' | sort | uniq -w 40 | cut -c 42-)
```

- 参考
  - https://qiita.com/yuba/items/852d019af48ee7ccd92e
