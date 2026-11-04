# ProxyIndicatorR

Windows の通知領域で手動プロキシの状態を確認し、アイコンの左クリックで ON／OFF を切り替えられます。自動検出、セットアップスクリプト、保存済みサーバー、除外一覧は保持します。

**[最新版をダウンロード](https://github.com/mezon-web/ProxyIndicatorR-Releases/releases/latest)**

## 起動する

1. Windows x64 に **.NET 10 Desktop Runtime（x64）** をインストールします。[Microsoft のダウンロードページ](https://dotnet.microsoft.com/ja-jp/download/dotnet/10.0)
2. Release の Assets から `ProxyIndicatorR-v0.1.1.zip` をダウンロードして展開します。
3. `ProxyIndicatorR-v0.1.1` フォルダーの `ProxyIndicatorR.exe` を起動します。同じフォルダーの `使い方.html` はオフラインで読めます。

## 操作する

- 緑の「PX」に一本の下線があれば手動プロキシ ON、橙の「PX」に左右に分かれた下線があれば OFF です。ポインターを重ねても状態を確認できます。
- 左クリックで、現在のユーザーの既定／LAN 接続を切り替えます。Windows の設定画面から変更した状態もアイコンに反映されます。
- 初回は Windows の「設定」→「ネットワークとインターネット」→「プロキシ」で手動サーバーのアドレスとポートを設定してください。
- 右クリック →「終了」で常駐を終了します。手動設定の最後の状態は保持されます。旧 Python 版を使っている場合は、先に終了してください。

## ダウンロードを確認する

Release から ZIP と同名の `.sha256` ファイルも取得できます。PowerShell で ZIP の SHA-256 を計算し、ファイルに記載された値と比較してください。

```powershell
Get-FileHash .\ProxyIndicatorR-v0.1.1.zip -Algorithm SHA256
```

[変更履歴](CHANGELOG.md) · [過去のリリース](https://github.com/mezon-web/ProxyIndicatorR-Releases/releases)
