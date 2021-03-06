# README

- data.json ... `aws stepfunctions get-execution-history` の戻り値（`nextToken` と `ExecutionStarted` の 1 イベントのみ）
- schema.json ... Get Execution history の戻り値の一部（`nextToken` と `events` を含む。 `events` は `ExecutionStarted` の 1 イベントのみ含むリスト型）

今回のスキーマ定義の `events` 配下にあるオブジェクト型を拡張して、他の Event type にも対応することで `GetExecutionHistory` API の戻り値をスキーマ定義することができる（はず）
