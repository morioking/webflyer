# webflyer

## 目的
うごくフライヤー

[ベルリン.club](http://xn--wdk8ac7a.club/)

## 要件
- 爆速で表示されること
- アニメーションなど画像だけのフライヤーと異なる表現をすること
- スマホ最適していること
- 紙や画像のフライヤーよりも、情報量で勝ること
- 紙や画像のフライヤーよりも、集客できること
- PC上でフルスクリーン表示できること（VJで使うことを想定）
- 8時間でコンテンツ作成できること
- アイキャッチが表示されること

## テックノート
- Bootstrap
- CreateJS
- [Google Fonts](https://fonts.google.com/)
- [AWS S3](https://console.aws.amazon.com/s3/home?region=us-west-2#&bucket=xn--wdk8ac7a.club&prefix=)
  - バケット名は xn--wdk8ac7a.club
- AWSのDNS
- Google analytics

## リポジトリ
https://github.com/morioking/webflyer.git


## 開発環境

### gitconfigの設定

~/.gitconfig に以下を書くとgraph表示がラク

```
[alias]
  lg = log --graph --pretty=format:'%Cred%h%Creset -%C(yellow)%d%Creset %s %Cgreen(%cr) %C(bold blue)<%an>%Creset' --abbrev-commit --date=relative
  lga = log --graph --all --pretty=format:'%Cred%h%Creset -%C(yellow)%d%Creset %s %Cgreen(%cr) %C(bold blue)<%an>%Creset' --abbrev-commit --date=relative
```
### AWS CLI
AWS CLI でファイルをアップロードする

#### インストール

[AWS CLI を使用してファイルを Amazon S3 にバックアップする](https://aws.amazon.com/jp/getting-started/tutorials/backup-to-s3-cli/)

#### サンプルコマンド

```
aws s3 cp index.html s3://xn--wdk8ac7a.club/
```

### OPG画像

#### OGP画像をog:imageで指定する

http://ogimage.tsmallfield.com/

https://ferret-plus.com/610

[OGPデバッガ](https://developers.facebook.com/tools/debug/sharing/)

#### OGP画像を確認する

http://seo-scene.com/ogp-image/

1200 x 630 px 以上推奨
最低でも 600 x 315 px、また大きければ大きいほど良いため 1200 x 630 px 以上の画像サイズが推奨されています。画像がクリッピングされるのを防ぐため、縦横比をなるべく1.91:1に近づけるようにしましょう。

