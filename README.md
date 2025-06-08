# learn-arm64-macos

Apple Silicon（M1／M2／M3／M4）上で、`vi`＋`as`＋`ld`だけを使って、CPUとダイレクトに対話できる力を身につけます。

---

##  目標

1. **基礎の基礎（0）**：アセンブリ言語の仕組み、レジスタ・メモリ・命令セットの理解  
2. **応用編（50）**：システムコール、スタック操作、分岐・ループ、文字列処理  
3. **到達点（100）**：パフォーマンス最適化、NEON（SIMD）利用、独自リンカ／デバッガ開発、簡易カーネルやブートローダの実装  

---

##  学習ロードマップ

| レッスン              | 内容                                       |
| --------------------- | ------------------------------------------ |
| **lesson00_intro**    | アセンブリとは？環境構築＆ツール紹介        |
| **lesson01_exit**     | 最小構成で `exit(0)` を実行                 |
| **lesson02_write**    | `write()` で “Hello, world!” を表示        |
| **lesson03_stack**    | スタック基礎：PUSH／POP、ローカル変数       |
| **lesson04_branch**   | 比較＆分岐、ループ制御                       |
| **lesson05_data**     | .data セクション、文字列・配列の扱い        |
| **lesson06_syscall**  | Linux vs macOS システムコールの違い        |
| **lesson07_optim**    | パイプライン意識の最適化、NOP除去          |
| **lesson08_neon**     | NEON SIMD 命令入門                         |
| **lesson09_linker**   | カスタムリンカスクリプトでセグメント配置    |
| **lesson10_boot**     | 簡易ブートローダ／カーネル起動              |

---

##  必要環境

- Apple Silicon（M1/M2/M3/M4）搭載の macOS  
- Xcode Command Line Tools（`xcode-select --install`）  
- 利用ツール：  
  - `vi`／`vim`  
  - `as`（Apple Assembler）  
  - `ld`（Apple Linker）  
  - `otool`, `hexdump`, `nm`, `strip`  

---

## 学習の心得
>手を動かしてこそ身につく。
小さなサンプルを自分で組み、解析し、改造してみよう。

- **本リポジトリは「CPUに近い視点」を身につけたいすべての人に贈ります。0から100まで、一歩一歩楽しみながら進めてください！**

