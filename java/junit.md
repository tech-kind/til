## 特定のパッケージのみテスト

- JUnitで特定のパッケージ（フォルダ）のみテストしたい場合
- `--tests`オプションを使用する

``` sh
$ ./gradlew win-ex-api:test --tests jp.co.xxxx.yyyy.zzzz.\*Test
```
