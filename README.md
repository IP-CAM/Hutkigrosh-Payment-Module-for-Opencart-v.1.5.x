## Module for integration with CMS OpenCart 1.5.x

This module provides interaction between the online store based on CMS Opencart version 1.5.x and the payment service hutkigrosh.by
  * Integration module for version [OpenCart 2.1.x] (https://github.com/esasby/hutkigrosh-opencart2.1-module)
  * Integration module for version [OpenCart 2.2.x] (https://github.com/esasby/hutkigrosh-opencart2.2-module)
  * Integration module for version [OpenCart 2.3.x] (https://github.com/esasby/hutkigrosh-opencart2.3-module)
  * Integration module for version [OpenCart 3.0.x] (https://github.com/esasby/hutkigrosh-opencart3.0-module)

### Installation Instructions:

1. Unzip the archive [opencart15-hutkigrosh-payment-module.zip] (https://github.com/esasby/hutkigrosh-opencart1.5-module/blob/master/opencart15-hutkigrosh-payment-module.zip) and copy all files to the server via FTP / SSH.
2. In the admin area of ​​OpenCart, select Extensions> Payments
3. Opposite the HutkiGrosh module, click "Install" and then "Change".
4. Fill in the parameters to identify your store in the HutkiGrosh system. The required fields are:
    * Unique identifier of the ERIP service - ID of the ERIP service
    * Login online store - login in the HutkiGrosh system.
    * Online store password - password in the HutkiGrosh system.
    * Path in the ERIP tree - the path for paying the invoice in the ERIP tree, which will be shown to the client after placing an order (for example, Payments> Store> Orders)
5. In the "Status" drop-down list, select "Enabled".
6. Save your changes.

### Attention!
To automatically update the status of the order (after the client pays the invoice issued to the ERIP), you must inform the technical support service of the "Hutki Grosh" service with the address of the processor:
``
http://mydomen.my/index.php?route=payment/hutkigrosh/notify
``

### Test data
To set up payment in test mode
 * use the data to connect to the test system obtained during registration in HutkiGrosh
 * enable the "Sandbox" mode in the module settings
 * to emulate the payment by the client of the invoice, use the personal account of the [test system] (https://trial.hgrosh.by) (menu _ ERIP payment test_)

_Developed and tested with OpenCart v.1.5.6.4
