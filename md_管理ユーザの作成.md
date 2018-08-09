───────────────────────────────────────────────────────────<br>
#### 基本仕様
１、APIパス：/addUsers<br>
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
|Location|https://dora.jpis.co.jp/Sales41_aws_demo/rest/UserInfoService/addUsers/担当者コード|

───────────────────────────────────────────────────────────<br>
#### レスポンスコンテント

|パラメータ名|説明|データ型|
|-|-|-|
|person_in_charge_name|担当者名|文字列|
|createDate|登録日時|日時|
|person_in_charge_code|担当者コード|文字列|

───────────────────────────────────────────────────────────<br>
#### リクエストサンプル（ID・PASSWORD認証）
curl -X POST \ <br>
 -H "user-id:demo@ebskk.com" \ <br>
 -H "user-key:11111111" \ <br>
 -H "Content-Type: application/json" \ <br>
 -d "{company_unique_code:12345678,person_in_charge_code:ebs@ebskk.com,passwords:ebs,person_in_charge_name:ebs,person_in_charge_mail:ebs@ebskk.com,mobile_tel:1234567890,home_tel:0987654321}" \ <br>
https://dora.jpis.co.jp/Sales41_aws_demo/rest/UserInfoService/addUsers <br>
───────────────────────────────────────────────────────────<br>
#### レスポンスサンプル（ID・PASSWORD認証）
HTTP/1.1 201 Created<br>
Content-Type: application/json;charset=UTF-8<br>
Location: https://dora.jpis.co.jp/Sales41_aws_demo/rest/UserInfoService/addUsers/担当者コード<br>

{"createDate":"2018-08-28T11:27:16.446Z","person_in_charge_name":"ebs","person_in_charge_code":"ebs@ebskk.com"}<br>
───────────────────────────────────────────────────────────<br>																																
