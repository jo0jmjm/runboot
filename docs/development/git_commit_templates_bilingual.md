# Git コミットメッセージテンプレート / Git Commit Message Templates

## 目次 / Table of Contents
1. [ファイルの操作 / File Operations](#ファイルの操作--file-operations)
2. [機能の変更 / Feature Changes](#機能の変更--feature-changes)
3. [バグ修正 / Bug Fixes](#バグ修正--bug-fixes)
4. [パフォーマンスとセキュリティ / Performance and Security](#パフォーマンスとセキュリティ--performance-and-security)
5. [ドキュメンテーションとテスト / Documentation and Testing](#ドキュメンテーションとテスト--documentation-and-testing)
6. [依存関係の管理 / Dependency Management](#依存関係の管理--dependency-management)
7. [リファクタリングとコード品質 / Refactoring and Code Quality](#リファクタリングとコード品質--refactoring-and-code-quality)
8. [バージョン管理とリリース / Version Control and Releases](#バージョン管理とリリース--version-control-and-releases)

## ファイルの操作 / File Operations

### ファイルの追加 / File Addition
* Add [ファイル名] for [目的]
  - 例: Add .gitignore for Node.js project
    - Node.jsプロジェクト用の.gitignoreを追加
* Create [ファイル名] to [目的]
  - 例: Create docker-compose.yml to set up local development environment
    - ローカル開発環境をセットアップするためのdocker-compose.ymlを作成

### ファイルの更新 / File Update
* Update [ファイル名] with [変更内容]
  - 例: Update user_schema.js with new email validation rules
    - 新しいメールバリデーションルールでuser_schema.jsを更新
* Modify [ファイル名] to [変更の目的]
  - 例: Modify webpack.config.js to optimize production build
    - プロダクションビルドを最適化するためにwebpack.config.jsを修正

### ファイルの削除 / File Deletion
* Remove [ファイル名] due to [理由]
  - 例: Remove deprecated_util.js due to refactoring of utility functions
    - ユーティリティ関数のリファクタリングにより、deprecated_util.jsを削除

## 機能の変更 / Feature Changes

### 機能の追加 / Feature Addition
* Implement [機能名]
  - 例: Implement two-factor authentication for user accounts
    - ユーザーアカウントの二要素認証を実装
* Add support for [新機能/技術]
  - 例: Add support for WebSocket connections in chat module
    - チャットモジュールにWebSocket接続のサポートを追加

### 機能の改善 / Feature Enhancement
* Enhance [機能名] with [改善内容]
  - 例: Enhance search functionality with fuzzy matching algorithm
    - あいまい一致アルゴリズムで検索機能を強化
* Extend [機能名] to [新しい機能]
  - 例: Extend user profile to include customizable avatars
    - カスタマイズ可能なアバターを含むようにユーザープロフィールを拡張

## バグ修正 / Bug Fixes

* Fix [問題の簡潔な説明]
  - 例: Fix memory leak in background worker process
    - バックグラウンドワーカープロセスのメモリリークを修正
* Resolve [問題] in [機能/ファイル]
  - 例: Resolve race condition in concurrent data access of user sessions
    - ユーザーセッションの並行データアクセスにおける競合状態を解決

## パフォーマンスとセキュリティ / Performance and Security

### パフォーマンス改善 / Performance Improvement
* Optimize [機能/プロセス] for [目的]
  - 例: Optimize database queries for faster dashboard loading
    - ダッシュボードの高速読み込みのためにデータベースクエリを最適化
* Improve performance of [機能] by [方法]
  - 例: Improve performance of image processing by implementing caching
    - キャッシュを実装することで画像処理のパフォーマンスを改善

### セキュリティ強化 / Security Enhancement
* Enhance security of [機能/プロセス]
  - 例: Enhance security of API endpoints with rate limiting
    - レート制限によりAPIエンドポイントのセキュリティを強化
* Implement [セキュリティ機能] for [目的]
  - 例: Implement CSRF protection for all form submissions
    - すべてのフォーム送信にCSRF保護を実装

## ドキュメンテーションとテスト / Documentation and Testing

### ドキュメンテーション / Documentation
* Update documentation for [機能/変更点]
  - 例: Update documentation for new API versioning system
    - 新しいAPIバージョニングシステムのドキュメントを更新
* Add [ドキュメントの種類] for [機能/コンポーネント]
  - 例: Add API documentation for user management endpoints
    - ユーザー管理エンドポイントのAPIドキュメントを追加

### テスト / Testing
* Add tests for [機能/コンポーネント]
  - 例: Add unit tests for date formatting utilities
    - 日付フォーマットユーティリティのユニットテストを追加
* Improve test coverage for [機能/モジュール]
  - 例: Improve test coverage for authentication middleware
    - 認証ミドルウェアのテストカバレッジを改善

## 依存関係の管理 / Dependency Management

* Upgrade [ライブラリ/フレームワーク] to [新バージョン]
  - 例: Upgrade React to version 18.0 for improved performance
    - パフォーマンス向上のためReactをバージョン18.0にアップグレード
* Replace [古いもの] with [新しいもの] for [理由]
  - 例: Replace Moment.js with date-fns for smaller bundle size
    - バンドルサイズ削減のためMoment.jsをdate-fnsに置き換え

## リファクタリングとコード品質 / Refactoring and Code Quality

* Refactor [コンポーネント/機能] for [目的]
  - 例: Refactor user authentication logic for better maintainability
    - 保守性向上のためユーザー認証ロジックをリファクタリング
* Improve code quality in [ファイル/モジュール]
  - 例: Improve code quality in data processing modules by applying SOLID principles
    - SOLIDの原則を適用してデータ処理モジュールのコード品質を改善

## バージョン管理とリリース / Version Control and Releases

* Prepare for release [バージョン番号]
  - 例: Prepare for release v1.2.0 with new user management features
    - 新しいユーザー管理機能を含むv1.2.0のリリース準備
* Merge branch [ブランチ名] into [ターゲットブランチ]
  - 例: Merge branch 'feature/oauth-integration' into develop
    - 'feature/oauth-integration'ブランチをdevelopブランチにマージ

---

注意: コミットメッセージは簡潔かつ明確に保ち、変更の理由や影響を含めるようにしてください。
長いメッセージが必要な場合は、1行目に要約を書き、空行を挟んで詳細を記述してください。

Note: Keep commit messages concise and clear, including the reason for the change and its impact.
For longer messages, write a summary in the first line, followed by a blank line and then the details.
