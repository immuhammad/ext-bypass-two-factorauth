# Overview #

In Magento 2.4.x, some merchants have trouble with two-factor authentications and want Magento’s previous behavior. By using PHP Studios Bypass2FA extension, selected admin users will have direct access to the admin dashboard without passing through the two- factor authentication process. So, the efficiency will be enhanced and admin stuff will speed up. In addition to that, this module helps to bypass 2FA for the integrations that use the default Magento’s API for token generation. All the Magento’s APIs which need Magento token as bearer needs admin token/integration token for calling APIs. This module gives the ability to generate the Admin Token without needing to go through tired some process of 2FA.

### Features ###

* Allow the merchant to bypass 2FA for selected admin users.
* Allow the merchant to re-enable 2FA at any time for the selected admin users.
* Provides facility to bypass 2FA for the third-party integrations that use the default Magento’s API for token generation such as Ship Station etc.
* Provides the facility to generate the Admin Token without needing to go through tired process of 2FA.
* Helps the merchant to keep using the integrations and make it compatible withMagento’s 2.4.x.
