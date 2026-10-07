# Verdant releases

macOS 版 Verdant の配布物(DMG)と、自動アップデート(Sparkle)の appcast を置くリポジトリ。
ソースコードは別のリポジトリにある。

- **初めて入れる人**: [Releases](../../releases/latest) から `Verdant-<version>-universal.dmg` を
  ダウンロードし、`Verdant.app` を「アプリケーション」フォルダへドラッグする。
  以降のアップデートはアプリが自動で行う(Verdant > アップデートを確認… でも確認できる)。
- **appcast.xml** は公開スクリプト(`scripts/macos/publish-update.sh`)が書き換える。手で編集しないこと
  (EdDSA で署名しているので、編集すると署名が合わなくなり、アプリが無視する)。
- このリポジトリは private。招待された人だけがダウンロードできる。アプリは
  このリポジトリだけを読める読み取り専用トークンを使って更新を取りに来る。
