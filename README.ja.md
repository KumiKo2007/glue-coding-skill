<p align="center">
  <a href="README.md">English</a> ·
  <a href="README.zh-CN.md">中文</a> ·
  <a href="README.ja.md"><strong>日本語</strong></a> ·
  <a href="README.ko.md">한국어</a>
</p>

<h1 align="center">glue-coding-skill：再発明せず、成熟した能力をつなぐ</h1>

<p align="center"><strong>Codex 用の Skill。成熟した SDK / API / フレームワーク / プラットフォーム機能を優先し、薄い glue code と品質ゲートで AI コーディングを安定させます。</strong></p>

<p align="center">
  <a href="LICENSE"><img alt="MIT" src="https://img.shields.io/badge/license-MIT-2ea44f?style=for-the-badge"></a>
  <img alt="Codex Skill" src="https://img.shields.io/badge/Codex-Skill-111827?style=for-the-badge">
  <img alt="AI Coding" src="https://img.shields.io/badge/AI%20Coding-Workflow-2563eb?style=for-the-badge">
</p>

## なぜ必要か

AI は大量のコードをすばやく生成できます。その一方で、認証、キュー、スケジューラ、ログ、ストレージ、SDK ラッパーなどを不用意に作り直してしまうことがあります。

`glue-coding` は Codex に次の判断軸を与えます。

> 共通問題は成熟した能力で解く。glue code は業務フローをつなぐ。独自実装はデフォルトではなく例外である。

## 何をしてくれるか

- 公式 SDK、API、マネージドサービス、安定した OSS を先に探す
- 保守状況、ドキュメント、ライセンス、セキュリティ、移行コストを評価する
- ドメインロジックと外部依存を分離する
- 短く、薄く、テスト可能で、削除しやすい glue code を促す
- テスト、schema、エラー処理、監視、ロールバック経路を確認する

## インストール

```powershell
git clone https://github.com/KumiKo2007/glue-coding-skill "$env:USERPROFILE\.codex\skills\glue-coding"
```

使い方：

```text
Use $glue-coding to design this feature with mature capabilities first.
```

## 向いている用途

- 機能設計
- アーキテクチャレビュー
- AI 生成コードのリファクタリング
- API / SDK 連携
- 作る・買う・包む・削除する判断

## License

MIT.