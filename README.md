# Common Tests Hyva MFTF3

<h4>Specific module for basic compatibility MFTF with Hyva.<h4>
<h2>Installation</h2>
<h4>Pre-conditions</h4>

 1. Install MFTF: <a>https://developer.adobe.com/commerce/testing/functional-testing-framework/getting-started/ <br>
   We recommend that you turn off the Magento_TwoFactorAuth module for ease of testing or configure credentials: <a>https://developer.adobe.com/commerce/testing/functional-testing-framework/two-factor-authentication/</a>
 2. Install and enable Hyva for global level:
    1. Install Hyva Theme: <a> https://docs.hyva.io/hyva-themes/getting-started/index.html </a>
    2. Open “Content -> Design -> Configuration” in Admin Area Magento Store.
    3. Choose “Global” Design Configuration and set “Default Hyva” in “Applied Theme” dropdown.
    4. Click to “Save Configuration”.
 3. Install and enable Hyva Luma Checkout: <a> https://docs.hyva.io/checkout/luma-checkout/installing-luma-checkout.html

<h4>Instruction</h4>
<p>To install the package, run the following commands:</p>
  <code>composer require amasty/module-common-tests-hyva-mftf-3</code><br>
  <code>php bin/magento setup:upgrade</code><br>
  <code>php bin/magento setup:di:compile </code><br>
  <code>php bin/magento setup:static-content:deploy (your locale)</code><br>

<h4>To run tests it is necessary</h4>
Run a special command for correct operation of the waits when you are running any tests <br><br>
<code>bin/magento amasty-mftf:hyva:waiting-update</code><br>

<h4>Run tests</h4>
<p>To run the tests, run the following command:</p>
Magento Commerce:<br>
<code>vendor/bin/mftf run:group AmDef -r</code><br><br>
Open Source Magento:<br>
<code>vendor/bin/mftf run:group AmDefCE -r</code><br>

<h2>Other Amasty extensions</h2>
-> <a href="https://amasty.com/multi-warehouse-inventory-for-magento-2.html" target="_blank">Multi Warehouse Inventory for Magento 2</a><br>
-> <a href="https://amasty.com/meta-tags-templates-for-magento-2.html" target="_blank">Meta Tags Templates for Magento 2</a><br>
-> <a href="https://amasty.com/mega-menu-for-magento-2.html" target="_blank">Mega Menu for Magento 2</a><br>
-> <a href="https://amasty.com/mass-product-actions-for-magento-2.html" target="_blank">Mass Product Actions for Magento 2</a><br>
-> <a href="https://amasty.com/mass-order-actions-for-magento-2.html" target="_blank">Mass Order Actions for Magento 2</a><br>
-> <a href="https://amasty.com/magento-2-upsell-cross-sell-extension.html" target="_blank">Cross-Sell / Upsell Products for Magento 2</a><br>
-> <a href="https://amasty.com/magento-2-order-status.html" target="_blank">Order Status for Magento 2</a><br>
-> <a href="https://amasty.com/magento-2-login-as-customer.html" target="_blank">Login as Customer for Magento 2</a><br>
-> <a href="https://amasty.com/magento-2-frequently-bought-together.html" target="_blank">Customers Also Bought for Magento 2</a><br>
-> <a href="https://amasty.com/magento-2-facebook-feed.html" target="_blank">Facebook Feed for Magento 2</a><br>
-> <a href="https://amasty.com/magento-2-custom-checkout-fields.html" target="_blank">Custom Checkout Fields for Magento 2</a><br>
-> <a href="https://amasty.com/loyalty-program-for-magento-2.html" target="_blank">Loyalty Program for Magento 2</a><br>
-> <a href="https://amasty.com/lite-layered-navigation-for-magento-2.html" target="_blank">Lite Layered Navigation for Magento 2</a><br>
-> <a href="https://amasty.com/lazy-load-for-magento-2.html" target="_blank">Lazy Load for Magento 2</a><br>
-> <a href="https://amasty.com/magento-seo-toolkit.html" target="_blank">SEO Toolkit</a><br>
-> <a href="https://amasty.com/magento-related-products.html" target="_blank">Automatic Related Products</a><br>
-> <a href="https://amasty.com/magento-loyalty-program.html" target="_blank">Loyalty Program</a><br>
-> <a href="https://amasty.com/magento-image-optimization-extension.html" target="_blank">Image Optimization</a><br>
