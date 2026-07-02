
# DB設計

## 概要

Learning Note v1では、学習メモと分類を管理する。

データはSQLiteに保存する想定とする。

---

## テーブル一覧

1. Categories
2. LearningNotes

---

## 1. Categories

分類を管理するテーブル。

| Column | Type | Description |
|---|---|---|
| Id | INTEGER | 主キー |
| Name | TEXT | 分類名 |
| CreatedAt | TEXT | 作成日時 |
| UpdatedAt | TEXT | 更新日時 |

---

## 2. LearningNotes

学習メモを管理するテーブル。

| Column | Type | Description |
|---|---|---|
| Id | INTEGER | 主キー |
| Title | TEXT | タイトル |
| Content | TEXT | 学習内容 |
| Memo | TEXT | 補足メモ |
| UnderstandingLevel | INTEGER | 理解度（1〜5） |
| CategoryId | INTEGER | 分類ID |
| CreatedAt | TEXT | 作成日時 |
| UpdatedAt | TEXT | 更新日時 |

---

## リレーション

LearningNotes.CategoryId は Categories.Id を参照する。

```text
Categories
   1
   │
   │
   N
LearningNotes
