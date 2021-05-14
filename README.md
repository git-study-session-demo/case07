# commitの様々なオプション

0. 準備
### フォークする
<img width="1435" alt="スクリーンショット 2021-05-15 3 35 28" src="https://user-images.githubusercontent.com/71377103/118317587-36a9f680-b533-11eb-8920-5303304fbc06.png">

### クローンする
<img width="1435" alt="スクリーンショット 2021-05-15 3 36 41" src="https://user-images.githubusercontent.com/71377103/118317604-3c074100-b533-11eb-8730-2ea509ef599f.png">

```
git clone <リポジトリURL>
```

### ブランチをきる
```
git switch -c feature/01
```

## -m
コミットメッセージをつける

## -a
変更されたファイルを検出し(新規に追加されたファイルを除く)、git add と git commit を同時に実行する。
```
echo 'Hello World!!' > sample.txt
```
```
git commit -am 'commit No.1'
```
```
git log
```
<img width="1435" alt="スクリーンショット 2021-05-15 4 00 08" src="https://user-images.githubusercontent.com/71377103/118317701-593c0f80-b533-11eb-9267-d073df5ad9e1.png">

## --amend
直前のコミットを上書きしてコミットする。
```
echo 'Change!!' > sample.txt
```
```
git commit --amend -am 'commit No.2'
```
```
git log
```
<img width="1435" alt="スクリーンショット 2021-05-15 4 01 25" src="https://user-images.githubusercontent.com/71377103/118317723-5f31f080-b533-11eb-95fb-10b7b12f7a0f.png">


