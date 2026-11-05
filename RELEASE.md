# リリース手順（自動アップデート配信）

このプラグインは同梱の Plugin Update Checker で GitHub リポジトリ
`terasakisd/alm-connector` のリリースを監視します。
**バージョンを上げてコミット・プッシュし、vX.Y.Z タグのリリースを作るだけで全サイトに配信されます。**

```bash
# 例: ヘッダの Version を上げてから
git add -A && git commit -m "vX.Y.Z: 変更内容" && git push
gh release create vX.Y.Z --title "vX.Y.Z" --notes "変更内容"
```
