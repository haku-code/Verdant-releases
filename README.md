# Verdant releases

macOS 版 Verdant の配布物(DMG)と、自動アップデート(Sparkle)の appcast を置くリポジトリ。
ソースコードは別の(非公開の)リポジトリにある。

- **初めて入れる人**: [Releases](../../releases/latest) から `Verdant-<version>-universal.dmg` を
  ダウンロードし、`Verdant.app` を「アプリケーション」フォルダへドラッグする。
  以降のアップデートはアプリが自動で行う(Verdant > アップデートを確認… でも確認できる)。
- **appcast.xml** は公開スクリプト(`scripts/macos/publish-update.sh`)と CI が書き換える。手で編集しないこと
  (EdDSA で署名しているので、編集すると署名が合わなくなり、アプリが無視する)。
- DMG は Developer ID で署名し、Apple の公証を受けている。更新ファイルは EdDSA 署名でも確かめる。
