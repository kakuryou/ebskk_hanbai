───────────────────────────────────────────────────────────<br>
#### 基本仕様
１、APIパス：/gaityusaki/企業標準コード/得意先コード/<br>
２、メソッド：GET<br>
───────────────────────────────────────────────────────────<br>
#### リクエストヘッダー
シグネチャやAPIキーなどの詳細は「共通フォーマット」を参照してください<br>

|フィールド名|内容|
|-|-|
|Content-Type|application/json|

───────────────────────────────────────────────────────────<br>
#### リクエストコンテント
なし<br>
───────────────────────────────────────────────────────────<br>
#### レスポンスHTTPステータス

|ステータスコード|説明|
|-|-|
|200|取得完了|

───────────────────────────────────────────────────────────<br>
#### レスポンスヘッダー

|フィールド名|値|
|-|-|
|Content-Type|application/json|

───────────────────────────────────────────────────────────<br>
#### レスポンスコンテント

|パラメータ名|説明|データ型|
|-|-|-|
|out_order_code|外注先コード|文字列|
|out_order_name|外注先名称|文字列|
|out_order_simple_name|外注先略称|文字列|
|out_order_fax|FAX|文字列|
|out_order_phone|電話番号|文字列|
|call_name|外注先区分|文字列|
|out_order_postcode|郵便番号|文字列|
|taxs_div|消費税区分|文字列|
|payment_date|支払日|文字列|
|fraction_processing|端数処理|文字列|
|payment_condition|支払条件|文字列|
|payment_delay_days|支払サイト|文字列|
|begin_buy_balance|期首買掛残高|文字列|
|last_payment_balance|前回支払残高|文字列|
|out_order_address1|外注先住所1|文字列|
|person_in_charge1|外注先担当者1|文字列|
|person_in_charge1_job|外注先担当者役職1|文字列|
|person_in_charge1_mail|外注先担当者メール1|文字列|
|bill_mail1|支払書宛先1|文字列|
|out_order_address2|外注先住所2|文字列|
|person_in_charge2|外注先担当者2|文字列|
|person_in_charge2_job|外注先担当者役職2|文字列|
|person_in_charge2_mail|外注先担当者メール2|文字列|
|bill_mail2|支払書宛先2|文字列|
|out_order_address3|外注先住所3|文字列|
|person_in_charge3|外注先担当者3|文字列|
|person_in_charge3_job|外注先担当者役職3|文字列|
|person_in_charge3_mail|外注先担当者メール3|文字列|
|bill_mail3|支払書宛先3|文字列|

───────────────────────────────────────────────────────────<br>
#### リクエストサンプル
curl -X GET -G \ <br>
 -H "user-id:demo@ebskk.com" \ <br>
 -H "user-key:11111111" \ <br>
 -H "Content-Type: application/json" \ <br>
https://dora.jpis.co.jp/Sales41_aws_demo/rest/UserInfoService/gaityusaki/12345678/000001 <br>
───────────────────────────────────────────────────────────<br>
#### レスポンスサンプル
{<br>
  "out_order_code":"000001",<br>
  "out_order_name":"得意先_ＥＢＳ_太郎_0000000001",<br>
  "out_order_simple_name":"名前0000000001",<br>
  "out_order_fax":"03-5339-1101  ",<br>
  "out_order_phone":null,<br>
  "call_name":null,<br>
  "out_order_postcode ":"03-5339-1102",<br>
  "taxs_div":"内税",<br>
  "fraction_processing":"切り捨て",<br>
  "payment_date":"20",<br>
  "payment_condition":"振込み",<br>
  "payment_delay_days":"10",<br>
  "begin_buy_balance":"100000",<br>
  "last_payment_balance":"50000",<br>
  "out_order_address1":"東京都",<br>
  "person_in_charge1":"太郎",<br>
  "person_in_charge1_job":"課長",<br>
  "person_in_charge1_mail":"admin@ebskk.com",<br>
  "bill_mail1":"admin@ebskk.com",<br>
  "out_order_address2":null,<br>
  "person_in_charge2":null,<br>
  "person_in_charge2_job":null,<br>
  "person_in_charge2_mail":null,<br>
  "bill_mail2":null,<br>
  "out_order_address3":null,<br>
  "person_in_charge3":null,<br>
  "person_in_charge3_job":null,<br>
  "person_in_charge3_mail":null,<br>
  "bill_mail3":null<br>
}<br>
───────────────────────────────────────────────────────────<br>
