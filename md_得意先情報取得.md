����������������������������������������������������������������������������������������������������������������������<br>
#### ��{�d�l
�P�AAPI�p�X�F/tokuisaki/��ƕW���R�[�h/���Ӑ�R�[�h/<br>
�Q�A���\�b�h�FGET<br>
����������������������������������������������������������������������������������������������������������������������<br>
#### ���N�G�X�g�w�b�_�[
�V�O�l�`����API�L�[�Ȃǂ̏ڍׂ́u���ʃt�H�[�}�b�g�v���Q�Ƃ��Ă�������<br>

|�t�B�[���h��|���e|
|-|-|
|Content-Type|application/json|
����������������������������������������������������������������������������������������������������������������������<br>
#### ���N�G�X�g�R���e���g
�Ȃ�<br>
����������������������������������������������������������������������������������������������������������������������<br>
#### ���X�|���XHTTP�X�e�[�^�X

|�X�e�[�^�X�R�[�h|����|
|-|-|
|200|�擾����|
����������������������������������������������������������������������������������������������������������������������<br>
#### ���X�|���X�w�b�_�[

|�t�B�[���h��|�l|
|-|-|
|Content-Type|application/json|
����������������������������������������������������������������������������������������������������������������������<br>
#### ���X�|���X�R���e���g

|�p�����[�^��|����|�f�[�^�^|
|-|-|-|
|customer_code|���Ӑ�R�[�h|������|
|customer_name|���Ӑ於��|������|
|customer_simple_name|���Ӑ旪��|������|
|customer_fax|FAX|������|
|customer_phone|�d�b�ԍ�|������|
|call_name|���Ӑ�敪|������|
|customer_postcode|�X�֔ԍ�|������|
|taxs_div|����ŋ敪|������|
|balance_date|����|������|
|fraction_processing|�[������|������|
|payment_date|������|������|
|payment_condition|��������|������|
|payment_delay_days|�����T�C�g|������|
|credit_sale_date|���|���|������|
|begin_sale_balance|���񔄊|�c��|������|
|last_claim_balance|�O�񐿋��c��|������|
|customer_address1|���Ӑ�Z��1|������|
|person_in_charge1|���Ӑ�S����1|������|
|person_in_charge1_job|���Ӑ�S���Җ�E1|������|
|person_in_charge1_mail|���Ӑ�S���҃��[��1|������|
|estimate_mail1|���ψ���1|������|
|bill_mail1|����������1|������|
|customer_address2|���Ӑ�Z��2|������|
|person_in_charge2|���Ӑ�S����2|������|
|person_in_charge2_job|���Ӑ�S���Җ�E2|������|
|person_in_charge2_mail|���Ӑ�S���҃��[��2|������|
|estimate_mail2|���ψ���2|������|
|bill_mail2|����������2|������|
|customer_address3|���Ӑ�Z��3|������|
|person_in_charge3|���Ӑ�S����3|������|
|person_in_charge3_job|���Ӑ�S���Җ�E3|������|
|person_in_charge3_mail|���Ӑ�S���҃��[��3|������|
|estimate_mail3|���ψ���3|������|
|bill_mail3|����������3|������|
����������������������������������������������������������������������������������������������������������������������<br>
#### ���N�G�X�g�T���v��
curl -X GET -G \ <br>
 -H "X-NCMB-Apps-Session-Token:46MnVgUbwHIXIHp9mowIeh7r2" \ <br>
 -H "X-NCMB-Application-Key: 549116a86b0ebbec4832d4086a56f36c82a5d64bc6528fa5e6220be76db5ef45" \ <br>
 -H "X-NCMB-Timestamp: 2013-08-14T15:46:25.543" \ <br>
 -H "X-NCMB-Signature: x2Dlg8KCZ7M77kD45ofeCZAJScVcVVl7Xn7SHhE0CF0=" \ <br>
 -H "Content-Type: application/json" \ <br>
https://hanbai.jpis.co.jp/rest/tokuisaki/12345678/000001<br>
����������������������������������������������������������������������������������������������������������������������<br>
#### ���X�|���X�T���v��
{<br>
  "customer_code":"000001",<br>
  "customer_name":"���Ӑ�_�d�a�r_���Y_0000000001",<br>
  "customer_simple_name":"���O0000000001",<br>
  "customer_fax":"03-5339-1101  ",<br>
  "customer_phone":null,<br>
  "call_name":null,<br>
  "customer_postcode ":"03-5339-1102",<br>
  "taxs_div":"����",<br>
  "balance_date":"99",<br>
  "fraction_processing":"�؂�̂�",<br>
  "payment_date":"20",<br>
  "payment_condition":"�U����",<br>
  "payment_delay_days":"10",<br>
  "credit_sale_date":"2018/01/01",<br>
  "begin_sale_balance":"100000",<br>
  "last_claim_balance":"50000",<br>
  "customer_address1":"�����s",<br>
  "person_in_charge1":"���Y",<br>
  "person_in_charge1_job":"�ے�",<br>
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
����������������������������������������������������������������������������������������������������������������������<br>
