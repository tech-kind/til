## 共有メモリ

- 共有メモリを使用してコントローラと他のプロセスを共有するサンプル
  - https://content.helpme-codesys.com/ja/CODESYS%20Examples/_ex_cds_shared_memory_communication.html

- 共有メモリを使用する際は`SysShm`ライブラリを参照する
  - `SysShm`について
  - https://content.helpme-codesys.com/en/libs/SysShm%20Implementation/Current/index.html
  - POSIXの名前付き共有メモリ
  - Linux環境の場合、/dev/shmに領域が確保される

## 排他・同期

- 共有メモリの排他制御・同期制御にはセマフォが利用可能
- セマフォを使用する際は`SysSemProcess`ライブラリを参照する
  - `SysSemProcess`について
  - https://content.helpme-codesys.com/en/libs/SysSemProcess/Current/index.html
  - POSIXの名前付きセマフォ
  - Linux環境の場合、/dev/shmに領域が確保される

