# README

JSONSchema の練習。

AWS Step Functions の [GetExecutionHistory](https://docs.aws.amazon.com/step-functions/latest/apireference/API_GetExecutionHistory.html#API_GetExecutionHistory_RequestSyntax) API の戻り値（の一部）を JSONSchema で検証する

- data.json ... `aws stepfunctions get-execution-history` の戻り値であるリスト型の 1要素（`ExecutionStarted` イベント）
- schema.json ... Execution history における `ExecutionStarted` イベントのスキーマ定義

## Usage

```bash
pip install -r requirements.txt

jsonschema -i data.json schema.json
```
