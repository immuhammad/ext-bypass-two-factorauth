<h1 align="center">Conequate_Bypass2FA</h1> 

<div align="center">
  <p>TIn Magento 2.4.x, some merchants have trouble with two-factor authentications and want Magento’s previous behavior. By using PHP Studios Bypass2FA extension, selected admin users will have direct access to the admin dashboard without passing through the two- factor authentication process. So, the efficiency will be enhanced and admin stuff will speed up. In addition to that, this module helps to bypass 2FA for the integrations that use the default Magento’s API for token generation. All the Magento’s APIs which need Magento token as bearer needs admin token/integration token for calling APIs. This module gives the ability to generate the Admin Token without needing to go through tired some process of 2FA.
</p>
  <img src="https://img.shields.io/badge/magento-2.2%20%7C%202.3%20%7C%202.4-brightgreen?logo=magento&longCache=true&style=flat-square" alt="Supported Magento Versions" />
  <a href="https://GitHub.com/Naereen/StrapDown.js/graphs/commit-activity" target="_blank"><img src="https://img.shields.io/badge/maintained%3F-yes-brightgreen.svg?style=flat-square" alt="Maintained - Yes" /></a>
  <a href="https://opensource.org/licenses/MIT" target="_blank"><img src="https://img.shields.io/badge/license-MIT-blue.svg" /></a>
</div>

## Table of contents

- [Feature](#feature)
- [Shared Package](#SharedPackage)
- [Installation](#installation)
- [License](#license)

## Feature

In the Bypass 2FA extension, merchants will have the ability to give permission to access the admin dashboard without passing through the two-factor authentication process to the specific admin users.

<ul>
<li>Log into the admin panel with default admin..</li>
<li>Click the Conequate admin dashboard menu item..</li>
<li>Beneath Bypass 2FA click Configuration.</li>
<li>You will be seeing a configuration containing all the admin users list.</li>
<li>Now, select the admin users to whom you want to bypass 2FA.</li>
<li>Click on Save Config to save the updated configurations.</li>
</ul>

Now, the selected admin users will not be going through the process of 2FA. To reverse the action, Unselect any selected admin user to enable 2FA again.

Now, unselected admins will be redirected to the process of 2FA. Allow the merchant to bypass 2FA for selected admin users.
- Allow the merchant to re-enable 2FA at any time for the selected admin users.
- Provides facility to bypass 2FA for the third-party integrations that use the default Magento’s API for token generation such as Ship Station etc.
- Provides the facility to generate the Admin Token without needing to go through tired process of 2FA.
- Helps the merchant to keep using the integrations and make it compatible with Magento’s 2.4.x.

## SharedPackage
There is a shared package (core module) associated with this extension having store configuration, menu items, and
logos. This extension expects to have a core module installed along/before with the extension as this extension has a
dependency on the Core module. `Conequate_Core` is free of cost.
The following command is to install `Conequate_Core` before installation of `Conequate_AddressAutoComplete`
module:

## Installation

```sh
composer require conequate/core
composer require conequate/bypass-two-factorauth
bin/magento module:enable Conequate_*
bin/magento setup:upgrade
```

### if your website is running in production mode you need to deploy static content and then clear the cache
```sh
php bin/magento setup:static-content:deploy
php bin/magento setup:di:compile
```

## License

[MIT](https://opensource.org/licenses/MIT)