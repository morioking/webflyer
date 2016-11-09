# webflyer

## 目的
動的フライヤー

[ベルリン.club](http://xn--wdk8ac7a.club/)

## 要件
- 爆速で表示されること
- アニメーションなど画像だけのフライヤーと異なる表現をすること
- スマホ最適していること
- 紙や画像のフライヤーよりも、情報量で勝ること
- 紙や画像のフライヤーよりも、集客できること
- PC上でフルスクリーン表示できること（VJで使うことを想定）
- 8時間でコンテンツ作成できること
- プレビューが表示されること

## 使用技術
- Bootstrap
- CreateJS
- [Google Fonts](https://fonts.google.com/)
- [AWS S3](https://console.aws.amazon.com/s3/home?region=us-west-2#&bucket=xn--wdk8ac7a.club&prefix=)
  - バケット名は xn--wdk8ac7a.club
- AWSのDNS
- Google analytics

## リポジトリ
[webflyer](https://github.com/morioking/webflyer.git)


## 開発環境

### gitconfigの設定

~/.gitconfig に以下を書くとgraph表示がラク

```
[alias]
  lg = log --graph --pretty=format:'%Cred%h%Creset -%C(yellow)%d%Creset %s %Cgreen(%cr) %C(bold blue)<%an>%Creset' --abbrev-commit --date=relative
  lga = log --graph --all --pretty=format:'%Cred%h%Creset -%C(yellow)%d%Creset %s %Cgreen(%cr) %C(bold blue)<%an>%Creset' --abbrev-commit --date=relative
```
