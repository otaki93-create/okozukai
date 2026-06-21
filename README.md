# お小遣い帳

毎月のお小遣い残高を管理するシンプルなWebアプリです。iPhoneのホーム画面に追加してアプリとして使えます。

## 機能

- 月ごとに予算を設定
- 支出を記録・削除
- 残高をリアルタイム表示（プログレスバー付き）
- 前後の月を切り替えて履歴を確認
- データはブラウザに自動保存（localStorage）

## 使い方

### GitHub Pages で公開する場合

1. このリポジトリをフォーク or クローン
2. GitHub の Settings → Pages → Branch: `main` / フォルダ: `/ (root)` で公開
3. 発行された URL を iPhone の Safari で開く

### iPhone のホーム画面に追加する方法

1. Safari でアプリのURLを開く
2. 画面下の共有ボタン（四角＋矢印）をタップ
3. 「ホーム画面に追加」を選択
4. 「追加」をタップ

これでアプリアイコンからフルスクリーンで起動できます。

## ファイル構成

```
okozukai-app/
├── index.html      # アプリ本体
├── icon.svg        # アプリアイコン
├── manifest.json   # PWA設定
└── README.md       # このファイル
```

## 技術仕様

- 純粋なHTML / CSS / JavaScript（フレームワーク不要）
- データ保存：localStorage（端末内のみ、サーバー送信なし）
- PWA対応（iPhoneホーム画面追加、フルスクリーン表示）
- Safe Area対応（iPhoneのノッチ・ホームバー考慮）
