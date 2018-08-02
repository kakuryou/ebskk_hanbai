───────────────────────────────────────────────────────────<br>
#### 基本仕様
１、APIパス：/tokuisaki/企業標準コード/得意先コード/<br>
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
|customer_code|得意先コード|文字列|
|customer_name|得意先名称|文字列|
|customer_simple_name|得意先略称|文字列|
|customer_fax|FAX|文字列|
|customer_phone|電話番号|文字列|
|call_name|得意先区分|文字列|
|customer_postcode|郵便番号|文字列|
|taxs_div|消費税区分|文字列|
|balance_date|締日|文字列|
|fraction_processing|端数処理|文字列|
|payment_date|入金日|文字列|
|payment_condition|入金条件|文字列|
|payment_delay_days|入金サイト|文字列|
|credit_sale_date|売掛基準日|文字列|
|begin_sale_balance|期首売掛残高|文字列|
|last_claim_balance|前回請求残高|文字列|
|customer_address1|得意先住所1|文字列|
|person_in_charge1|得意先担当者1|文字列|
|person_in_charge1_job|得意先担当者役職1|文字列|
|person_in_charge1_mail|得意先担当者メール1|文字列|
|estimate_mail1|見積宛先1|文字列|
|bill_mail1|請求書宛先1|文字列|
|customer_address2|得意先住所2|文字列|
|person_in_charge2|得意先担当者2|文字列|
|person_in_charge2_job|得意先担当者役職2|文字列|
|person_in_charge2_mail|得意先担当者メール2|文字列|
|estimate_mail2|見積宛先2|文字列|
|bill_mail2|請求書宛先2|文字列|
|customer_address3|得意先住所3|文字列|
|person_in_charge3|得意先担当者3|文字列|
|person_in_charge3_job|得意先担当者役職3|文字列|
|person_in_charge3_mail|得意先担当者メール3|文字列|
|estimate_mail3|見積宛先3|文字列|
|bill_mail3|請求書宛先3|文字列|

───────────────────────────────────────────────────────────<br>
#### リクエストサンプル
curl -X GET -G \ <br>
 -H "user-key:11111111" \ <br>
 -H "Content-Type: application/json" \ <br>
https://dora.jpis.co.jp/Sales41_aws_demo/rest/UserInfoService/tokuisaki/12345678/000001<br>
───────────────────────────────────────────────────────────<br>
#### レスポンスサンプル
{<br>
  "customer_code":"000001",<br>
  "customer_name":"得意先_ＥＢＳ_太郎_0000000001",<br>
  "customer_simple_name":"名前0000000001",<br>
  "customer_fax":"03-5339-1101  ",<br>
  "customer_phone":null,<br>
  "call_name":null,<br>
  "customer_postcode ":"03-5339-1102",<br>
  "taxs_div":"内税",<br>
  "balance_date":"99",<br>
  "fraction_processing":"切り捨て",<br>
  "payment_date":"20",<br>
  "payment_condition":"振込み",<br>
  "payment_delay_days":"10",<br>
  "credit_sale_date":"2018/01/01",<br>
  "begin_sale_balance":"100000",<br>
  "last_claim_balance":"50000",<br>
  "customer_address1":"東京都",<br>
  "person_in_charge1":"太郎",<br>
  "person_in_charge1_job":"課長",<br>
  "person_in_charge1_mail":"admin@ebskk.com",<br>
  "estimate_mail1":"admin@ebskk.com",<br>
  "bill_mail1":"admin@ebskk.com",<br>
  "customer_address2":null,<br>
  "person_in_charge2":null,<br>
  "person_in_charge2_job":null,<br>
  "person_in_charge2_mail":null,<br>
  "estimate_mail2":null,<br>
  "bill_mail2":null,<br>
  "customer_address3":null,<br>
  "person_in_charge3":null,<br>
  "person_in_charge3_job":null,<br>
  "person_in_charge3_mail":null,<br>
  "estimate_mail3":null,<br>
  "bill_mail3":null<br>
}<br>
───────────────────────────────────────────────────────────<br>
