# クラス設計

## 概要

Learning Note v1で使用するクラスを定義する。

---

# LearningNote

学習メモを表すクラス。

## プロパティ

| 名前 | 型 | 説明 |
|------|----|------|
| Id | int | メモID |
| Title | string | タイトル |
| Content | string | 学習内容 |
| Memo | string | 補足メモ |
| UnderstandingLevel | int | 理解度 |
| CategoryId | int | 分類ID |
| CreatedAt | DateTime | 作成日時 |
| UpdatedAt | DateTime | 更新日時 |

---

# Category

分類を表すクラス。

## プロパティ

| 名前 | 型 | 説明 |
|------|----|------|
| Id | int | 分類ID |
| Name | string | 分類名 |
| CreatedAt | DateTime | 作成日時 |
| UpdatedAt | DateTime | 更新日時 |

---

# 関連

Category

↓

LearningNote

1対多

1つの分類には複数の学習メモを登録できる。
