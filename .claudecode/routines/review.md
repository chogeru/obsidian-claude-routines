# name: weekly-schedule-sync

## 目的
Google Calendarの予定を読み取り、ウィークリーノートを更新してリポジトリにPushする。

## 手順
1. **[Connector: Google Calendar]** を使用して、今日から1週間の予定を取得してください。
2. リポジトリ内の `CalendarSchedule` ディレクトリを確認し、今週のファイル（例: 2026-W20.md）を特定してください。ディレクトリがなければ作成してください。
3. 既存のユーザーメモを保持したまま、予定部分のみを差分更新してください。
4. **必須アクション**: 更新完了後、ターミナルで `git add .` → `git commit -m "Auto-update schedule"` → `git push` を確実に実行してGitHubに変更を保存してください。