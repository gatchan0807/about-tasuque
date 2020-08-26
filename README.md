# About タスクエ

https://タスクエ.com のアプリについての概要紹介用リポジトリ（バグ・Secrets等問題ないか確認前で、コード公開準備中のため）

![ロゴ](https://storage.googleapis.com/studio-design-assets/projects/BRO3b2J0WD/s-512x512_webp_036c31e0-c802-4efa-98eb-de71d88b1542.webp)

# URL

- アプリケーション本体: https://タスクエ.com
- LP・使い方解説用ページ: https://tasque-lp.studio.design/

# 使用技術

## 技術系
- Nuxt [2.13.0]
- Tailwind CSS
- Firebase
  - Firebase Auth
  - Firestore
  - Firebase Hosting
- AVA（まだ一つも書けていない）

## アセット系
- Fortawesome
- Freepik

## ツール系

- Figma（ロゴ・OGP等作成）
- STUDIO（LP・使い方ページ作成）

# ゲーミフィケーションについて参考にしたもの

- [メンタリストDaiGoさん](https://twitter.com/Mentalist_DaiGo)が解説していたゲーミフィケーションについての[論文解説・考察動画](https://www.nicovideo.jp/watch/so37088143)
  - 上記をベースに、自分がシュミレーションゲームが好きなのでポイントを「貯める」というエッセンスを追加してベースを作成

# ディレクトリ構成

## Pages

```
pages
├── account.vue
├── base-quest.vue
├── config.vue
├── index.vue
├── punishment-game.vue
├── reward.vue
└── today.vue
```

## Component
```
components
├── atoms
│   └── headerMenuItem.vue
├── molecules
│   ├── dialogButton.vue
│   ├── diceShuffleButton.vue
│   ├── questFormRow.vue
│   ├── signpost.vue
│   └── topCardUserData.vue
└── organisms
    ├── accountMenu.vue
    ├── configOfBaseQuests.vue
    ├── configOfPunishmentGames.vue
    ├── configOfRewards.vue
    ├── configTemplates.vue
    ├── dialog.vue
    ├── dialogForm.vue
    ├── dice.vue
    ├── formDialog.vue
    ├── header.vue
    ├── table.vue
    └── todayQuestForm.vue
```

## Store

```
store
├── account.js
├── actionLog.js
├── config.js
├── index.js
├── points.js
├── punishment.js
└── today.js
```

## Plugin

```
plugins
├── dialog.js
├── firebase.js
├── font-awesome.js
└── vee-validate.js
```
