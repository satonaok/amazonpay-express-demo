#IntroductionLogin and Pay with Amazon provides millions of buyers a secure, trusted, and convenient way to pay fortheir purchases on your site. To complete their purchase, buyers simply select a shipping address andpayment method stored in their Amazon Payments account.  #####Custom integration can be used in the following scenarios                                           * If your parameters will change dynamically on the checkout page and cannot be preloaded.* If you have a multiitem shopping cart.* if your store contains multiple items wherein using static buttons for each item is not feasible. #####Scope of the Examples                                                                           * Examples are showcased in languages such as `PHP`, `C#`, `Java`, `Ruby`.* A simple cart page with Item name and Quantity.* The [dynamic parameters](~Dynamic Parameters) are passed to the backend and the signature is calculated.* Signature is appended to a data-structure along with the other parameters and encoded in JSON.* The JSON encoded String is then passed through the Javascript in the Front End.* The checkout process begins once the signature and the other required input parameters are verified.#Getting Started                                                                                To use the Pay with Amazon button you will need the following:                              1.	Register with Amazon Payments                                                           2.	Download this project as a zip or clone the project#Dynamic Parameters#####1. `amount`The amount of the payment.##### 2. `sellerNote`The message that will appear in the checkout pages.(Max length: 1024 characters)#####3. `sellerOrderId`The seller specified identifier of this order. This is displayed in buyer emails and in the transaction history on the Amazon Payments website.                                                             We recommend that you use the following characters only: lowercase a-z, uppercase A-Z, numbers 0-9, dash (-), or underscore (_).Max length: 50 characters                                                           #####4. `currencyCode`The currency to use to charge the buyer.                                                        Default: current seller region                                                                  Example: USD