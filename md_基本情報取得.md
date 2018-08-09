───────────────────────────────────────────────────────────<br>
#### 基本仕様
１、APIパス：/base/企業標準コード<br>
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
|company_name|会社名|文字列|
|company_english_name|会社英文名|文字列|
|zip_code|郵便番号|文字列|
|phone1|電話番号|文字列|
|phone2|電話番号|文字列|
|phone3|電話番号|文字列|
|fax|FAX|文字列|
|mail_address|メールアドレス|文字列|
|manager|代表名|文字列|
|tax_rates|税率|文字列|
|bank_no|銀行口座|文字列|
|home_page|ホームページ|文字列|
|address|会社住所|文字列|
|year_period_start|年度期間|文字列|
|year_period_end|年度期間|文字列|
|company_unique_code|企業標準コード|文字列|

───────────────────────────────────────────────────────────<br>
#### リクエストサンプル
curl -X GET -G \ <br>
 -H "user-id:demo@ebskk.com" \ <br>
 -H "user-key:11111111" \ <br>
 -H "Content-Type: application/json" \ <br> 
https://dora.jpis.co.jp/Sales41_aws_demo/rest/UserInfoService/base/12345678 <br>
───────────────────────────────────────────────────────────<br>
#### レスポンスサンプル
{<br>
  "company_name":"株式会社eビジネスソリューション",<br>
  "company_english_name":"  EBS",<br>
  "zip_code":"163-0636",<br>
  "phone1":"03-5339-1101  ",<br>
  "phone2":null,<br>
  "phone3":null,<br>
  "fax ":"03-5339-1102",<br>
  "mail_address":"info@edc.co.jp",<br>
  "manager":null,<br>
  "tax_rates":"5",<br>
  "bank_no":"1234567890",<br>
  "home_page":"www.edic.co.jp",<br>
  "address":"東京都新宿区西新宿1-25-1新宿センタービル36F",<br>
  "year_period_start":"2018/1/1",<br>
  "year_period_end":"2018/12/31",<br>
  "company_unique_code":"12345678"<br>
}<br>
───────────────────────────────────────────────────────────<br>
