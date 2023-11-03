## opencart-3-payment-module

### Installation

* Backup your webstore and database
* Upload the module file opencart-3-assetpayments-payment-module.ocmod.zip via Extensions -> Extension Installer
* Activate the module in payment extensions (Extensions -> Payments)
* Configure the module settings:
  * User Id
  * Secret key
  * Template ID 
  * Order statuses for successfuly processed payment
  * Enabled the module
  * And optionally setup sort order id if you want to move the payment option higher level in payment method list
  
### Notes
Tested and developed with OpenCart v.3.0.2.0

### Set products language
Add this before product array
* $this->load->language('product/product');
* $language_id = 2; // Language ID
* $this->config->set('config_language_id', $language_id);

### Troubleshooting
Alternatively you can just upload the upload directory content to your opencart installation directory.

## Модуль оплаты OpenCart 3

### Установка
* Создайте резервную копию вашего магазина и базы данных
* Загрузите файл модуля opencart-3-assetpayments-payment-module.ocmod.zip с помощью Модули -> Установка расширений
* Активируйте модуль AssetPayments в модулях оплаты (Модули -> Оплата)
* Задайте в настройках модуля:
  * Id магазина
  * Ключ магазина
  * Id шаблона
  * Статусы заказа в случае успешной и не успешной оплаты
  * Включите модуль
  * Опционально задайте идентификатор модуля для сортировки его в списке способов оплаты. Меньшее значение подымает модуль в верх списка

### Примечания
Разработано и протестировано с OpenCart v.3.0.2.0

### Проблемы при установке
Другой вариант - это закачать на сервер содержимое папки upload в корень директoрии, где устанвлена OpenCart
