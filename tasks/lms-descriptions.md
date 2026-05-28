# LMS概要欄インデックス（プロンプト・公式リンク）

LMS（AI+）の各レクチャー概要欄に貼り付けるファイルとリンクを動画単位で整理。
プロンプトはすべて **`.md` ファイルとして各動画フォルダに配置済み**。LMSの「ファイルをドラッグ&ドロップ」機能で添付してアップロードする。

- `[ ]` を `[x]` にしてアップ済みを管理する
- ファイル本文を更新したいときは、該当 `.md` を直接編集する。このインデックスはリンクのみ持つ
- 新しいプロンプトを追加するときは、該当動画フォルダに `prompt-NN-内容.md` を作って、ここにエントリを足す

---

## サービス公式リンク集（共通）

各動画の概要欄に必要に応じて貼る。**収録時／アップロード時に必ず実機で開いてリダイレクト先・最新URLを確認すること**（公式サイトはサインアップフローを更新することがある）。

| サービス | 想定貼付URL | どの動画で使う |
|---|---|---|
| Claude Code（デスクトップ版ダウンロード） | `https://claude.com/download` | S1V3 |
| GitHub（サインアップ） | `https://github.com/signup` | S5V1 |
| Vercel（サインアップ） | `https://vercel.com/signup` | S5V2 |
| Supabase（トップ／サインアップ） | `https://supabase.com` | S6V1〜V3 |
| Notion（サインアップ） | `https://www.notion.so/signup` | S4V3（Notion MCP回） |
| Slack（サインアップ） | `https://slack.com/get-started` | S4V3（Slack MCP回） |

---

## S1V3 — Claude Code デスクトップ版のインストール

- [ ] LMSにアップロード済み
- 種別: **リンクのみ**（プロンプトなし）
- 台本該当箇所: [s1v3/script.md:22](s1v3/script.md:22)

**貼る内容**: Claude Code 公式ダウンロードページのURL（上の公式リンク集を参照）

---

## S3V1 — 確定申告Skillで学ぶ Agent Skills の極意

- [ ] LMSにアップロード済み
- 種別: **リンク＋注記**（コマンド一覧・公式リンクは概要欄に記載済み）
- 公式リンク: Agent Skills サンプル・仕様集 https://github.com/anthropics/skills
- 台本該当箇所: [s3v1/script.md:54](s3v1/script.md:54)（「（Claude Code CLIを起動）」）

**概要欄に追記する注記**（受講生FBより。S1V3はデスクトップ版アプリのインストールのみ案内しており、本動画が使う Claude Code CLI のインストールが未案内。ターミナルで `claude` が `command not found: claude` になる）:

> 【はじめに｜Claude Code CLI のインストール（重要）】
>
> この動画の実演では「Claude Code CLI」（ターミナルで claude コマンドを実行する版）を使用します。S1V3でインストールしたデスクトップ版アプリとは別物で、CLIはアプリとは別にインストールが必要です。
>
> ※ ChatGPT等で「Node.js が必要」と案内される場合がありますが、現在の公式手順では Node.js は不要です。
>
> ▼ Mac の場合：ターミナル（Terminal.app）で以下を実行（Anthropic 公式インストーラ）
>
> curl -fsSL https://claude.ai/install.sh | bash
>
> ▼ インストール後の動作確認：
>
> claude --version
>
> バージョン番号（例：2.1.144）が出れば成功。「command not found: claude」が出た場合は、Claude Code デスクトップ版の Code タブに次を貼り付けると自動で直せる：
>
> 「Macのターミナルで claude --version を実行すると command not found: claude が出る状態を解消し、claude --version でバージョンが表示されるところまで進めてください。すでに curl -fsSL https://claude.ai/install.sh | bash は実行済みです。~/.local/bin がPATHに通っていないのが原因と思われます。私のシェルと現状のPATHを確認したうえで、適切な設定ファイル（.zshrc等）に追記してください。編集前にバックアップを取ってください。」

> 根本対応メモ: 再収録時は [s3v1/script.md:54](s3v1/script.md:54)「（Claude Code CLIを起動）」の直前に、CLI インストール手順（curl ワンライナー＋ `claude --version` 確認＋PATH追加）を台本へ畳み込む。それまでは上の概要欄注記が橋渡し。

---

## S4V1 — 【人事向け】社内eラーニングシステムを自作しよう

- [ ] LMSにアップロード済み
- 添付ファイル: [s4v1/prompt-01-spec.md](s4v1/prompt-01-spec.md)
- 台本該当箇所: [s4v1/script.md:43](s4v1/script.md:43)

---

## S4V2 — 【バックオフィス向け】勤怠の突き合わせチェックを自動化しよう

- [ ] LMSにアップロード済み
- 添付ファイル: [s4v2/prompt-01-report.md](s4v2/prompt-01-report.md)
- 台本該当箇所: [s4v2/script.md:29](s4v2/script.md:29)

---

## S4V3 — 【経営者向け】Slack・Notion MCPから週次サマリー自動生成しよう

- [ ] LMSにアップロード済み
- 添付ファイル: [s4v3/prompt-01-summary.md](s4v3/prompt-01-summary.md)
- 公式リンク: Notion・Slack のサインアップURL（上記表参照）
- 台本該当箇所: [s4v3/script.md:41](s4v3/script.md:41)

---

## S4V4 — 【マーケティング向け】高品質SEO記事を分割工程で生成しよう

- [ ] LMSにアップロード済み
- 添付ファイル: [s4v4/prompt-01-seo.md](s4v4/prompt-01-seo.md)
- 台本該当箇所: [s4v4/script.md:45](s4v4/script.md:45)

---

## S5V1 — GitHub入門 アカウント作成と初めてのリポジトリ

- [ ] LMSにアップロード済み
- 添付ファイル: [s5v1/prompt-01-repo.md](s5v1/prompt-01-repo.md)
- 公式リンク: GitHub サインアップURL（上記表参照）
- 台本該当箇所: [s5v1/script.md:53](s5v1/script.md:53)

**概要欄に追記する注記**（受講生FBより。動画は `gh` インストール済み前提のため、未インストール環境で `gh auth login` がエラーになる）:

> 【補足】`gh auth login` の前に GitHub CLI のインストールが必要です
>
> この動画ではターミナルで `gh auth login` を実行します。これには GitHub CLI（`gh` コマンド）が事前にインストールされている必要があり、未インストールの環境では `gh auth login` がエラーになります。
>
> `gh auth login` に進む前に、Claude Code に次のように頼んでください。お使いのパソコン（Mac / Windows）に合わせて Claude Code がインストールします。
>
> 「GitHub CLI（gh コマンド）をインストールしてください」
>
> うまく伝わらないときは、次の公式ページのURLもあわせて Claude Code に渡してください。Claude Code がページを読んで、環境に合った手順でインストールします。
>
> （参考）GitHub CLI 公式ページ: https://cli.github.com/
>
> インストールが完了したら、動画の手順どおり `gh auth login` から続けてください。

> 根本対応メモ: 再収録時は [s5v1/script.md:45](s5v1/script.md:45) の `gh auth login` 実行前に `gh` インストール手順を台本へ畳み込む。それまでは上の概要欄注記が橋渡し。

---

## S5V2 — Vercel入門 アカウント作成と初めてのデプロイ

- [ ] LMSにアップロード済み
- 添付ファイル: [s5v2/prompt-01-html.md](s5v2/prompt-01-html.md)
- 公式リンク: Vercel サインアップURL（上記表参照）
- 台本該当箇所: [s5v2/script.md:31](s5v2/script.md:31)

---

## S5V4 — 名刺管理アプリのフロントエンドをスペック駆動で作ろう

- [ ] LMSにアップロード済み
- 添付ファイル: [s5v4/prompt-01-design.md](s5v4/prompt-01-design.md)（CLAUDE.md / spec.md 設計プロンプト）
- 台本該当箇所: [s5v4/script.md:40](s5v4/script.md:40)

---

## S5V5 — 経費管理アプリのフロントエンドをスペック駆動で作ろう

- [ ] LMSにアップロード済み
- 添付ファイル: [s5v5/prompt-01-design.md](s5v5/prompt-01-design.md)（CLAUDE.md / spec.md 設計プロンプト）
- 台本該当箇所: [s5v5/script.md:40](s5v5/script.md:40)

---

## S5V6 — 顧客管理アプリのフロントエンドをスペック駆動で作ろう

- [ ] LMSにアップロード済み
- 添付ファイル: [s5v6/prompt-01-design.md](s5v6/prompt-01-design.md)（CLAUDE.md / spec.md 設計プロンプト）
- 台本該当箇所: [s5v6/script.md:40](s5v6/script.md:40)

---

## S6V1 — 名刺管理アプリにデータベースを接続して永続化しよう

- [ ] LMSにアップロード済み
- 添付ファイル（3本）:
  - [s6v1/prompt-01-table.md](s6v1/prompt-01-table.md) — Supabaseテーブル定義SQL生成
  - [s6v1/prompt-02-supabase.md](s6v1/prompt-02-supabase.md) — Vite導入＋Supabase接続
  - [s6v1/prompt-03-template.md](s6v1/prompt-03-template.md) — 自分のアプリ用 汎用テンプレート
- 公式リンク: Supabase（上記表参照）
- 台本該当箇所: [s6v1/script.md:44](s6v1/script.md:44) / [s6v1/script.md:75](s6v1/script.md:75) / [s6v1/script.md:118](s6v1/script.md:118)

---

## S6V2 — 経費管理アプリにデータベースを接続して集計しよう

- [ ] LMSにアップロード済み
- 添付ファイル（2本）:
  - [s6v2/prompt-01-table.md](s6v2/prompt-01-table.md) — Supabaseテーブル定義＋集計用RPC関数のSQL生成
  - [s6v2/prompt-02-supabase.md](s6v2/prompt-02-supabase.md) — Vite導入＋Supabase接続＋集計ボタン実装
- 公式リンク: Supabase（上記表参照）
- 台本該当箇所: [s6v2/script.md:42](s6v2/script.md:42) / [s6v2/script.md:62](s6v2/script.md:62)

---

## S6V3 — 顧客管理アプリにデータベースを接続してリレーション設計をしよう

- [ ] LMSにアップロード済み
- 添付ファイル（2本）:
  - [s6v3/prompt-01-table.md](s6v3/prompt-01-table.md) — 2テーブル分のSupabaseテーブル定義SQL生成
  - [s6v3/prompt-02-supabase.md](s6v3/prompt-02-supabase.md) — Vite導入＋Supabase接続＋リレーション取得
- 公式リンク: Supabase（上記表参照）
- 台本該当箇所: [s6v3/script.md:56](s6v3/script.md:56) / [s6v3/script.md:72](s6v3/script.md:72)

---

## メンテナンス指針

- 新動画を作って台本に「概要欄に貼っておきます」を含めたら、**同じコミット**で該当動画フォルダに `prompt-NN-内容.md` を作り、このインデックスにエントリを追加する
- プロンプト本文を編集するときは、各 `prompt-NN-*.md` を直接修正する（このファイルはリンクだけなので追従不要）
- 概要欄添付の有無を grep で再確認するときは: `grep -rn "概要欄" --include="*.md" .`
- 公式URLは収録／アップロード時に必ず実機で開いて最新フローを確認する
