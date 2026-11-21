# detect_meteors_assets

RAW image sequences, labels, and checksums for [detect_meteors](https://github.com/shin3tky/detect_meteors).

## Download RAW images / RAW 画像の取得

Install Git LFS to download the RAW images. The commands below clone the
repository without downloading the RAW images, then fetch only
`2024GEMINI_AIRCRAFT`.

RAW 画像の取得には Git LFS が必要です。次のコマンドでは RAW 画像の自動取得をスキップしてクローンし、`2024GEMINI_AIRCRAFT` だけを取得します。

```bash
git lfs install --skip-repo
GIT_LFS_SKIP_SMUDGE=1 git clone https://github.com/shin3tky/detect_meteors_assets.git
cd detect_meteors_assets
git lfs pull --include='rawfiles/2024GEMINI_AIRCRAFT/**'
```

To fetch a different sequence, replace `2024GEMINI_AIRCRAFT` in the
`--include` path. If you already have a clone, run the `git lfs pull`
command from its root.

別の系列を取得するには、`--include` のパス内の系列名を置き換えてください。クローン済みの場合は、そのリポジトリのルートで `git lfs pull` を実行してください。

## Sequences / 系列

Each sequence README lists its labels and checksum verification instructions.
各系列の README にラベルとチェックサムの確認手順があります。

- [2021GEMINI](rawfiles/2021GEMINI/README.md)
- [2024GEMINI](rawfiles/2024GEMINI/README.md)
- [2024GEMINI_AIRCRAFT](rawfiles/2024GEMINI_AIRCRAFT/README.md)
