───────────────────────────────────────────────────────────<br>
#### 基本仕様
１、APIパス：/users<br>
２、メソッド：POST<br>
───────────────────────────────────────────────────────────<br>
#### リクエストヘッダー
シグネチャやAPIキーなどの詳細は「共通フォーマット」を参照してください。<br>

|フィールド名|内容|
|-|-|
|Content-Type|application/json|

───────────────────────────────────────────────────────────<br>
#### リクエストコンテント

|パラメータ名|説明|データ型|必須|チェック|
|-|-|-|-|-|
|company_unique_code|企業標準コード|文字列、半角50桁|△|存在チェック|
|person_in_charge_code|担当者コード|文字列、半角60桁|△|一意チェック、フォーマットチェック|
|passwords|パスワ―ド|文字列、半角50桁|△||
|person_in_charge_name|担当者名|文字列、半角20桁|△||
|person_in_charge_mail|担当者メールアドレス|文字列、半角60桁|△|フォーマットチェック|
|mobile_tel|携帯電話番号|文字列、半角20桁|||
|home_tel|自宅電話番号|文字列、半角20桁|||

───────────────────────────────────────────────────────────<br>
#### レスポンスHTTPステータス

|ステータスコード|説明|
|-|-|
|200|登録完了|

───────────────────────────────────────────────────────────<br>
#### レスポンスヘッダー

|フィールド名|値|
|-|-|
|Content-Type|application/json|
|Location|https://XXXXXXX.com/rest/users/担当者コード|

───────────────────────────────────────────────────────────<br>
#### レスポンスコンテント

|パラメータ名|説明|データ型|
|-|-|-|
|person_in_charge_name|担当者名|文字列|
|createDate|登録日時|日時|
|sessionToken|セッショントークン|文字列|
|person_in_charge_code|担当者コード|文字列|

───────────────────────────────────────────────────────────<br>
#### リクエストサンプル（ID・PASSWORD認証）
curl -X POST \ <br>
 -H "X-Application-Key: 549116a86b0ebbec4832d4086a56f36c82a5d64bc6528fa5e6220be76db5ef45" \ <br>
 -H "X-Timestamp: 2018-08-14T15:46:25.543" \ <br>
 -H "X-Signature: l2ljScCsh1/oPv7mYePjUNPEDI81s85PYCT7ciTaiVM=" \ <br>
 -H "Content-Type: application/json" \ <br>
 -d '{"company_unique_code": "12345678", "person_in_charge_code": "admin@ebskk.com","passwords":"admin","person_in_charge_name":"ebskk","person_in_charge_mail":"admin@ebskk.com","mobile_tel":"1234567890","home_tel":"0987654321"}' \ <br>
https://hanbai.jpis.co.jp/rest/users <br>
───────────────────────────────────────────────────────────<br>
#### レスポンスサンプル（ID・PASSWORD認証）
HTTP/1.1 201 Created<br>
Content-Type: application/json;charset=UTF-8<br>
Location: http://hanbai.jpis.co.jp/rest/users/担当者コード<br>

{"createDate":"2018-08-28T11:27:16.446Z","person_in_charge_name":"ebskk","sessionToken":"iXDIelJRY3ULBdms281VTmc5O","person_in_charge_code":"admin@ebskk.com"}<br>
───────────────────────────────────────────────────────────<br>																																
