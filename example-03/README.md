# README

- data.json ... `aws stepfunctions get-execution-history` の戻り値
- schema.json ... Get Execution history の戻り値（`events` に含むイベントタイプは `ExecutionStarted` , `executionSucceeded` の 2 種類のみ想定）

## note

`array` タイプの `items` のスキーマ定義において、 `anyOf` と `oneOf` をそれぞれ以下のように解釈されるので注意

- anyOf ... その array オブジェクトの**各要素**は、 anyOf で列挙した定義のうちいずれかの型を持つ
- oneOf ... その array オブジェクトの**全要素**は、 anyOf で列挙した定義のいずれか1つの型を持つ

array に含まれる各要素について、すべての要素が同じ型を持つことを強制したい場合は `oneOf` を使用する。

array に含まれる各要素の型が単一でなくともよく、特定の型定義のうちいずれかに合致していればよい場合は `anyOf` を使う。
