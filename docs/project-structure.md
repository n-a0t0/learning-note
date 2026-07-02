# プロジェクト構成

## フォルダ構成

```text
LearningNote

├── Models
├── Views
├── ViewModels
├── Services
├── Data
├── Resources
├── Helpers
├── docs
└── README.md
```

---

## Models

データを表すクラスを配置する。

例

- LearningNote.cs
- Category.cs

---

## Views

画面を配置する。

例

- MainWindow.xaml
- NoteEditView.xaml
- NoteDetailView.xaml
- CategoryView.xaml

---

## ViewModels

画面とデータをつなぐ処理を書く。

例

- MainViewModel.cs
- NoteEditViewModel.cs

---

## Services

機能をまとめる。

例

- NoteService.cs
- SearchService.cs

将来

AIService.cs

もここへ追加する。

---

## Data

SQLiteやEntity Framework Coreを管理する。

例

- AppDbContext.cs

---

## Resources

画像やアイコンを配置する。

---

## Helpers

共通処理を書く。

例

- DateTimeHelper.cs
```
