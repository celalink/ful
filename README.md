# おすすめサイト一覧

MkDocs + Material で運用するリンク集です。
外部の方からの **Pull Request（PR）歓迎**です。

## 動作環境

OS:Mac OS (Sequoia 15.6.1)
Python:3.11.1

## ローカルでの動作確認手順

- Python 仮想環境を作成して有効化（推奨）

```bash
# macOS / Linux
python -m venv .venv
source .venv/bin/activate

# Windows (PowerShell)
py -m venv .venv
.\.venv\Scripts\Activate.ps1
```

- 依存パッケージをインストール

```bash
pip install -r requirements.txt
```

- ローカルで起動して確認

```bash
mkdocs serve
```

ブラウザで http://127.0.0.1:8000 を開く

## 編集ガイド

- サイトの追加提案は Pull Request でお願いします
- リポジトリとForkしてご利用ください
- PR の際にはサイトのジャンルをコメントで説明してください
- ローカル環境で編集後の画面キャプチャをPull Requestに追加して頂けると助かります

## よくある質問（FAQ）

Q. 事前に何を入れればいい？
A. Python（3.9+ 推奨）さえあればOK。pip install -r requirements.txt で必要なものは全部入ります。

Q. 依存関係は固定してる？
A. はい。requirements.txt にバージョンを固定しています。再現性のため勝手に上げないでください（上げるPRは歓迎。別PRで）。

Q. ローカルプレビューができません
A. まず仮想環境が有効か確認 → pip list に mkdocs と mkdocs-material が見えるかをチェック。ポート競合なら mkdocs serve -a 127.0.0.1:8001 を試してください。
