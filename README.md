# README

JSONSchema の練習。

AWS Step Functions の [GetExecutionHistory](https://docs.aws.amazon.com/step-functions/latest/apireference/API_GetExecutionHistory.html#API_GetExecutionHistory_RequestSyntax) API の戻り値（の一部）を JSONSchema で検証する

## Usage

```bash
pip install -r requirements.txt

jsonschema -i data.json schema.json
```
