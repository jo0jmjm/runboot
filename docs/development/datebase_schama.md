# runboot データベーススキーマ初期設計

## 目次
1. [概要](#1-概要)
2. [テーブル構造](#2-テーブル構造)
3. [関連図](#3-関連図)
4. [注意事項](#4-注意事項)

## 1. 概要
本文書は、runbootプロジェクトのデータベーススキーマの初期設計を定義します。このスキーマは、ユーザー管理、コース管理、学習進捗追跡などの主要機能をサポートするように設計されています。

## 2. テーブル構造

### 2.1 Users テーブル
- id (主キー)
- username
- email
- password_hash
- created_at
- updated_at

### 2.2 Courses テーブル
- id (主キー)
- title
- description
- language
- level
- created_at
- updated_at

### 2.3 Lessons テーブル
- id (主キー)
- course_id (外部キー、Coursesテーブルを参照)
- title
- content
- order
- created_at
- updated_at

### 2.4 UserProgress テーブル
- id (主キー)
- user_id (外部キー、Usersテーブルを参照)
- lesson_id (外部キー、Lessonsテーブルを参照)
- status
- completed_at

### 2.5 Projects テーブル
- id (主キー)
- course_id (外部キー、Coursesテーブルを参照)
- title
- description
- requirements
- created_at
- updated_at

### 2.6 UserProjects テーブル
- id (主キー)
- user_id (外部キー、Usersテーブルを参照)
- project_id (外部キー、Projectsテーブルを参照)
- submission_content
- status
- submitted_at
- reviewed_at

### 2.7 Resources テーブル
- id (主キー)
- course_id (外部キー、Coursesテーブルを参照)
- title
- url
- type
- created_at
- updated_at

## 3. 関連図
[ER図をここに挿入]

## 4. 注意事項
- このスキーマは初期設計であり、プロジェクトの進行に伴って変更される可能性があります。
- 実装時には、インデックスの追加、適切なデータ型の選択、正規化レベルの調整を行ってください。
- パフォーマンスとスケーラビリティを考慮し、必要に応じてデータベースの分割やシャーディングを検討してください。
- セキュリティを確保するため、特に個人情報を含むフィールドには適切な暗号化措置を講じてください。
