## 成果物紹介

### ハザードマップの実装と情報可視化アプリ

- 時期：2021.9

- 背景
  - 株式会社ウェザーニューズ　防災チャットボットコース5daysインターン
  - チーム開発

- 技術
  - フロントエンド：TypeScript/React.js
  - インフラ：AWS

- 概要
  - react-leafletライブラリを使ってハザードマップの実装に取り組み、特定の場所をマーカーで表示できるようにしました。
  - パフォーマンスの改善面では、マーカーを個別のDOM要素として追加するのではなく、代わりに静的なCanvasにレンダリングするようにしました。
  - なお、下記の図に示したように、AWSのCloud9で開発を行い、CodeCommitでバージョン管理を行いました。
  - その後、生成したSDKなどの必要なファイルをS3に投げ、Cloudfrontでデプロイしました。
  - この一連の作業を自動化させるために、シェルスクリプトを用いてCI/CDの作成を工夫しました。

<div align="center">
<img alt="開発の流れ" src="fig/map_flow.png" width="50%">
</div>

アプリの全体像

https://user-images.githubusercontent.com/63705408/148248365-0201f728-fc1a-4049-a3c6-4880dd7eb52f.mov

パフォーマンス改善前

https://user-images.githubusercontent.com/63705408/148247557-ce16709f-6977-4a90-a39b-36791fbecf28.mov

パフォーマンス改善後

https://user-images.githubusercontent.com/63705408/148248424-f2b573ef-4117-49fb-bc79-e248f4470b0e.mov


