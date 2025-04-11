# SimpleAlarmClock

シンプルかつ高機能なマルチアラームアプリケーションです。  
HTML、CSS、JavaScript を使用して実装されており、ユーザーが指定した条件に応じたアラームを設定できます。  
ブラウザの localStorage を利用して設定情報を永続化するため、ページ再読み込み後もアラーム設定が保持されます。

## デモページ

[https://c-a-p-engineer.github.io/SimpleAlarmClock/](https://c-a-p-engineer.github.io/SimpleAlarmClock/)

## 特徴

- **多彩なアラームタイプ**  
  - **毎日アラーム**: 毎日指定した時刻にアラーム発動  
  - **曜日指定アラーム**: 指定した曜日にアラーム発動  
  - **一回限りアラーム**: 指定した日付と時刻で一度だけアラーム発動

- **有効／無効切替**  
  - 各アラームを有効・無効に切り替えることができます。  
  - 無効にしたアラームは発動せず、再設定可能です。

- **時報機能**  
  - 1時間毎に時報（チマ音）を鳴らす機能を搭載。  
  - ユーザーが時報機能の有効・無効を切り替えることが可能です。

- **永続保存機能**  
  - ローカルストレージ（localStorage）を利用してアラーム設定を保存。  
  - ページの再読み込みやブラウザの再起動後も設定情報が保持されます。

- **シンプルでクールな UI**  
  - ダークトーンを基調としたモダンなデザイン。  
  - 設定済みアラームは、次回実行時刻の昇順に並び替えられ、視認しやすくなっています。

## 使い方

1. **アラームの設定**  
   - 画面上部の設定エリアで「時刻入力」欄にアラーム時刻を設定してください。  
   - アラームタイプ（毎日、曜日指定、一回限り）を選択し、必要に応じて追加のオプション（チェックボックスや日付選択）で詳細を指定します。  
   - 「アラーム追加」ボタンをクリックすると、設定内容が一覧に追加されます。

2. **有効／無効の切り替え**  
   - 設定済みアラーム一覧の「有効」列にあるチェックボックスで、各アラームの有効／無効を切り替えることができます。  
   - 無効にしたアラームは、次回実行時刻になっても音が鳴りません。

3. **時報機能**  
   - 設定エリア下部の「時報機能を有効にする (1時間毎)」のチェックボックスで、1時間毎の時報機能を有効化できます。  
   - 有効にすると、毎正時に指定の音声ファイルが再生されます。

4. **アラーム発動と停止**  
   - 設定されたアラーム時刻に到達すると、アラーム用音声（`zunda_time.wav`）がループ再生されます。  
   - 発動中は「アクティブアラーム」エリアが表示され、【停止】ボタンをクリックするとアラームが停止します。

5. **設定の永続化**  
   - アラーム設定や時報機能の状態は自動的にブラウザに保存されるため、再読み込み後も設定内容が復元されます。

## 導入方法

1. このリポジトリをクローン、または ZIP ダウンロードしてください。

   ```bash
   git clone https://github.com/c-a-p-engineer/SimpleAlarmClock.git
   ```

2. クローンしたディレクトリ内に `index.html` と同一階層に `zunda_time.wav` を配置します。

3. お好みのブラウザで `index.html` を開いて、アラームの動作を確認してください。

## カスタマイズ

- アラーム用および時報用の音声ファイルは、`zunda_time.wav` をご用意ください。  
  必要に応じて、異なる音声ファイルに差し替えることも可能です。
- UI のデザインや機能追加は、コード内の HTML/CSS/JavaScript を編集することで行えます。

## ライセンス

このプロジェクトは [MIT License](LICENSE) のもとで公開されています。

---

ご不明な点があれば、Issue や Pull Request をご利用ください。
