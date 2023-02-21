---
# multilingual page pair id, this must pair with translations of this page. (This name must be unique)
lng_pair: id_What_is_this
title: "コマンドの使い方"

# post specific
# if not specified, .name will be used from _data/owner/[language].yml
author: rkcyk706
# multiple category is not supported
category: Tips
# multiple tag entries are possible
tags: [Tips]
# thumbnail image for post
img: ":2023-02-21_17.54.58.png"
# disable comments on this page
#comments_disable: true

# publish date
date: 2023-02-20 22:50:00 +0900

# seo
# if not specified, date will be used.
#meta_modify_date: 2023-02-20 18:00:00 +0900
# check the meta_common_description in _data/owner/[language].yml
#meta_description: ""

# optional
# please use the "image_viewer_on" below to enable image viewer for individual pages or posts (_posts/ or [language]/_posts folders).
# image viewer can be enabled or disabled for all posts using the "image_viewer_posts: true" setting in _data/conf/main.yml.
#image_viewer_on: true
# please use the "image_lazy_loader_on" below to enable image lazy loader for individual pages or posts (_posts/ or [language]/_posts folders).
# image lazy loader can be enabled or disabled for all posts using the "image_lazy_loader_posts: true" setting in _data/conf/main.yml.
#image_lazy_loader_on: true
# exclude from on site search
#on_site_search_exclude: true
# exclude from search engines
#search_engine_exclude: true
# to disable this page, simply set published: false or delete this file
#published: false
---

![幽世ゲート](2023-02-21_17.54.58.png "幽世ゲート"){: .img-responsive}

# コマンド一覧

- [テレポート(TP)](#tp)
  
  - [公共TP](#public_tp)
  - [プレイヤー間TP](#player_tp)

- [その他のコマンド](#misc_command)

- [管理者コマンド](#admin_command)
  
  - [チャンク事前生成](#chunk_pregen)

## テレポート(TP) <a id="tp"></a>

| コマンド                  | 説明               |
| --------------------- | ---------------- |
| `/home`               | 設定した場所に移動します。    |
| `/sethome <name>`     | 移動先を設定します。       |
| `/delhome <name>`     | 移動先の設定を削除します。    |
| `/listhomes <player>` | 設定した場所を一覧に表示します。 |

## 公共TP <a id="public_tp"></a>

| コマンド           | 説明               |
| -------------- | ---------------- |
| `/spawn`       | 初期スポーンに移動します。    |
| `/warp <name>` | 設定された場所に移動します    |
| `/setwarp`     | 移動先を設定します。       |
| `/delwarp`     | 移動先の設定を削除します。    |
| `/listwarps`   | 設定した場所を一覧に表示します。 |

## プレイヤー間TP <a id="player_tp"></a>

| コマンド                | 説明                            |
| ------------------- | ----------------------------- |
| `/tpa <player>`     | 相手プレイヤーにTPするためにTPを申請します。      |
| `/tpshere <player>` | 相手プレイヤーに自分の所へTPするようにTPを要請します。 |
| `/tpaccept <id>`    | 申請・要請を受け入れます。(画面にボタンが表示されます)  |
| `/tpadeny <id>`     | 申請・要請を拒否します。(画面にボタンが表示されます)   |

# その他のコマンド <a id="misc_command"></a>

| コマンド          | 説明                           |
| ------------- | ---------------------------- |
| `/kickme`     | 自分をサーバーから追い出します。             |
| `/trashcan`   | アイテムを入れて閉じると削除されるイベントリを開きます。 |
| `/hat`        | 持ってるアイテムやブロックを頭にかぶります。       |
| `/hat <name>` | チャットのニックネームを変更します。           |

# 管理者コマンド <a id="admin_command"></a>

## チャンク事前生成 <a id="chunk_pregen"></a>

| コマンド                              | 説明                                |
| --------------------------------- | --------------------------------- |
| `/chunky start`                   | 新しいチャンク生成を開始します。                  |
| `/chunky pause`                   | 現在のタスクを一時停止し進捗を保存します。             |
| `/chunky continue`                | 現在のタスクまたは保存されたタスクの実行を維持します。       |
| `/chunky cancel`                  | 現在のタスクを停止し進捗をキャンセルします。            |
| `/chunky world [world]`           | 現在選択されているワールドを設定します。              |
| `/chunky shape <shape>`           | 生成する形状を指定します。                     |
| `/chunky center [<x> <y>]`        | 現在のセンターブロックの位置を指定します。             |
| `/chunky radius <radius>`         | 現在の半径を指定します。                      |
| `/chunky worldborder`             | 選択されたワールドの境界線に一致するように中心と半径を設定します。 |
| `chunky spawn`                    | 中心のスポーンポイントを設定します。                |
| `chunky corners <x1><z1><x2><z2>` | コーナー座標で選択範囲を指定します。                |
| `chunky pattern <pattern>`        | 生成パターンを設定します。                     |
| `chunky selection`                | 現在の指定範囲を表示します。                    |
| `chunky silent`                   | 更新のお知らせのオン・オフを切り替えます。             |
| `chunky quiet <interval>`         | 更新のお知らせを非表示にする時間を秒単位で設定します。       |
| `chunky progress`                 | ゲーム内のタスクについて、生成前の進捗状況を表示します。      |
| `chunky reload`                   | 設定を再読み込みします。                      |
| `chunky trim`                     | 範囲指定外のチャンクを削除します。                 |
