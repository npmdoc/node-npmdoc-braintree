# api documentation for  [braintree (v2.0.2)](http://github.com/braintree/braintree_node)  [![npm package](https://img.shields.io/npm/v/npmdoc-braintree.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-braintree) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-braintree.svg)](https://travis-ci.org/npmdoc/node-npmdoc-braintree)
#### A library for integrating with Braintree.

[![NPM](https://nodei.co/npm/braintree.png?downloads=true)](https://www.npmjs.com/package/braintree)

[![apidoc](https://npmdoc.github.io/node-npmdoc-braintree/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-braintree_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-braintree/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-braintree/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-braintree/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Braintree",
        "email": "code@braintreepayments.com",
        "url": "http://www.braintreepayments.com"
    },
    "bugs": {
        "url": "https://github.com/braintree/braintree_node/issues"
    },
    "dependencies": {
        "dateformat": "1.0.1-1.2.3",
        "depd": "~1.1.0",
        "readable-stream": "1.1.10",
        "semver": "5.1.0",
        "source-map-support": "0.2.9",
        "underscore": "1.8.3",
        "xml2js": "0.1.13"
    },
    "description": "A library for integrating with Braintree.",
    "devDependencies": {
        "chai": "1.5.0",
        "coffee-script": "1.6.1",
        "eslint": "^2.7.0",
        "eslint-config-braintree": "^1.0.2",
        "mocha": "3.2.0"
    },
    "directories": {
        "lib": "./lib"
    },
    "dist": {
        "shasum": "3c898c40404969f34d31e158fe0b17c09d7955f5",
        "tarball": "https://registry.npmjs.org/braintree/-/braintree-2.0.2.tgz"
    },
    "engines": {
        "node": ">=4"
    },
    "gitHead": "d2e1e52d8bb702f1de261d7ecd4b9165ddaf0436",
    "homepage": "http://github.com/braintree/braintree_node",
    "keywords": [
        "braintree",
        "payments"
    ],
    "license": "MIT",
    "main": "index",
    "maintainers": [
        {
            "name": "braintree",
            "email": "devs@getbraintree.com"
        }
    ],
    "name": "braintree",
    "optionalDependencies": {
        "source-map-support": "0.2.9"
    },
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/braintree/braintree_node.git"
    },
    "scripts": {
        "lint": "eslint lib/",
        "test": "npm run lint && npm run test:unit",
        "test:integration": "mocha --timeout 60000 --slow 2000 spec/integration --recursive --compilers coffee:coffee-script",
        "test:unit": "mocha spec/unit --recursive --compilers coffee:coffee-script"
    },
    "version": "2.0.2"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module braintree](#apidoc.module.braintree)
1.  [function <span class="apidocSignatureSpan">braintree.</span>AmexExpressCheckoutCard (attributes)](#apidoc.element.braintree.AmexExpressCheckoutCard)
1.  [function <span class="apidocSignatureSpan">braintree.</span>AndroidPayCard (attributes)](#apidoc.element.braintree.AndroidPayCard)
1.  [function <span class="apidocSignatureSpan">braintree.</span>ApplePayCard (attributes)](#apidoc.element.braintree.ApplePayCard)
1.  [function <span class="apidocSignatureSpan">braintree.</span>CoinbaseAccount (attributes)](#apidoc.element.braintree.CoinbaseAccount)
1.  [function <span class="apidocSignatureSpan">braintree.</span>CreditCard ()](#apidoc.element.braintree.CreditCard)
1.  [function <span class="apidocSignatureSpan">braintree.</span>CreditCardVerification ()](#apidoc.element.braintree.CreditCardVerification)
1.  [function <span class="apidocSignatureSpan">braintree.</span>Environment ()](#apidoc.element.braintree.Environment)
1.  [function <span class="apidocSignatureSpan">braintree.</span>MerchantAccount ()](#apidoc.element.braintree.MerchantAccount)
1.  [function <span class="apidocSignatureSpan">braintree.</span>PayPalAccount (attributes)](#apidoc.element.braintree.PayPalAccount)
1.  [function <span class="apidocSignatureSpan">braintree.</span>Subscription ()](#apidoc.element.braintree.Subscription)
1.  [function <span class="apidocSignatureSpan">braintree.</span>TestingGateway (gateway)](#apidoc.element.braintree.TestingGateway)
1.  [function <span class="apidocSignatureSpan">braintree.</span>Transaction ()](#apidoc.element.braintree.Transaction)
1.  [function <span class="apidocSignatureSpan">braintree.</span>ValidationErrorCodes ()](#apidoc.element.braintree.ValidationErrorCodes)
1.  [function <span class="apidocSignatureSpan">braintree.</span>VenmoAccount (attributes)](#apidoc.element.braintree.VenmoAccount)
1.  [function <span class="apidocSignatureSpan">braintree.</span>WebhookNotification ()](#apidoc.element.braintree.WebhookNotification)
1.  [function <span class="apidocSignatureSpan">braintree.</span>connect (new Config(config)](#apidoc.element.braintree.connect)
1.  object <span class="apidocSignatureSpan">braintree.</span>PaymentInstrumentTypes
1.  object <span class="apidocSignatureSpan">braintree.</span>Test
1.  object <span class="apidocSignatureSpan">braintree.</span>errorTypes
1.  string <span class="apidocSignatureSpan">braintree.</span>version



# <a name="apidoc.module.braintree"></a>[module braintree](#apidoc.module.braintree)

#### <a name="apidoc.element.braintree.AmexExpressCheckoutCard"></a>[function <span class="apidocSignatureSpan">braintree.</span>AmexExpressCheckoutCard (attributes)](#apidoc.element.braintree.AmexExpressCheckoutCard)
- description and source-code
```javascript
class AmexExpressCheckoutCard extends AttributeSetter {
  constructor(attributes) {
    super(attributes);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.braintree.AndroidPayCard"></a>[function <span class="apidocSignatureSpan">braintree.</span>AndroidPayCard (attributes)](#apidoc.element.braintree.AndroidPayCard)
- description and source-code
```javascript
class AndroidPayCard extends AttributeSetter {
  constructor(attributes) {
    super(attributes);

    if (attributes) {
      this.cardType = attributes.virtualCardType;
      this.last4 = attributes.virtualCardLast4;
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.braintree.ApplePayCard"></a>[function <span class="apidocSignatureSpan">braintree.</span>ApplePayCard (attributes)](#apidoc.element.braintree.ApplePayCard)
- description and source-code
```javascript
class ApplePayCard extends AttributeSetter {
  constructor(attributes) {
    super(attributes);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.braintree.CoinbaseAccount"></a>[function <span class="apidocSignatureSpan">braintree.</span>CoinbaseAccount (attributes)](#apidoc.element.braintree.CoinbaseAccount)
- description and source-code
```javascript
class CoinbaseAccount extends AttributeSetter {
  constructor(attributes) {
    super(attributes);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.braintree.CreditCard"></a>[function <span class="apidocSignatureSpan">braintree.</span>CreditCard ()](#apidoc.element.braintree.CreditCard)
- description and source-code
```javascript
class CreditCard extends AttributeSetter {
  static initClass() {
    this.CardType = {
      AmEx: 'American Express',
      CarteBlanche: 'Carte Blanche',
      ChinaUnionPay: 'China UnionPay',
      DinersClubInternational: 'Diners Club',
      Discover: 'Discover',
      JCB: 'JCB',
      Laser: 'Laser',
      Maestro: 'Maestro',
      MasterCard: 'MasterCard',
      Solo: 'Solo',
      Switch: 'Switch',
      Visa: 'Visa',
      Unknown: 'Unknown',
      All() {
        let all = [];

        for (let key in this) {
          if (!this.hasOwnProperty(key)) {
            continue;
          }
          let value = this[key];

          if (key !== 'All') { all.push(value); }
        }
        return all;
      }
    };

    this.CustomerLocation = {
      International: 'international',
      US: 'us'
    };

    this.CardTypeIndicator = {
      Yes: 'Yes',
      No: 'No',
      Unknown: 'Unknown'
    };

    this.Prepaid = this.Commercial = this.Payroll = this.Healthcare = this.DurbinRegulated =
      this.Debit = this.CountryOfIssuance = this.IssuingBank = this.ProductId = this.CardTypeIndicator;
  }

  constructor(attributes) {
    super(attributes);
    this.maskedNumber = '${this.bin}******${this.last4}';
    this.expirationDate = '${this.expirationMonth}/${this.expirationYear}';
    if (attributes) {
      let sortedVerifications = (attributes.verifications || []).sort((a, b) => b.created_at - a.created_at);

      if (sortedVerifications[0]) { this.verification = new CreditCardVerification(sortedVerifications[0]); }
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.braintree.CreditCardVerification"></a>[function <span class="apidocSignatureSpan">braintree.</span>CreditCardVerification ()](#apidoc.element.braintree.CreditCardVerification)
- description and source-code
```javascript
class CreditCardVerification extends AttributeSetter {
  static initClass() {
    this.StatusType = {
      Failed: 'failed',
      GatewayRejected: 'gateway_rejected',
      ProcessorDeclined: 'processor_declined',
      Verified: 'verified',
      All() {
        let all = [];

        for (let key in this) {
          if (!this.hasOwnProperty(key)) {
            continue;
          }
          let value = this[key];

          if (key !== 'All') { all.push(value); }
        }
        return all;
      }
    };
  }

  constructor(attributes) {
    super(attributes);
    if (attributes.riskData) { this.riskData = new RiskData(attributes.riskData); }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.braintree.Environment"></a>[function <span class="apidocSignatureSpan">braintree.</span>Environment ()](#apidoc.element.braintree.Environment)
- description and source-code
```javascript
class Environment {
  static initClass() {
    DEVELOPMENT_PORT = process.env.GATEWAY_PORT || '3000';
    this.Development = new Environment('localhost', DEVELOPMENT_PORT, 'http://auth.venmo.dev:9292', false);
    this.Qa = new Environment('gateway.qa.braintreepayments.com', '443', 'https://auth.venmo.qa2.braintreegateway.com', true);
    this.Sandbox = new Environment('api.sandbox.braintreegateway.com', '443', 'https://auth.sandbox.venmo.com', true);
    this.Production = new Environment('api.braintreegateway.com', '443', 'https://auth.venmo.com', true);
  }

  constructor(server, port, authUrl, ssl) {
    this.server = server;
    this.port = port;
    this.authUrl = authUrl;
    this.ssl = ssl;
  }

  baseUrl() {
    let url = this.uriScheme() + this.server;

    if (this === Environment.Development) {
      url += ':${this.port}';
    }

    return url;
  }

  uriScheme() {
    return this.ssl ? 'https://' : 'http://';
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.braintree.MerchantAccount"></a>[function <span class="apidocSignatureSpan">braintree.</span>MerchantAccount ()](#apidoc.element.braintree.MerchantAccount)
- description and source-code
```javascript
class MerchantAccount extends AttributeSetter {
  static initClass() {
    this.Status = {
      Pending: 'pending',
      Active: 'active',
      Suspended: 'suspended'
    };

    this.FundingDestination = {
      Bank: 'bank',
      Email: 'email',
      MobilePhone: 'mobile_phone'
    };
  }

  constructor(attributes) {
    super(attributes);
    if (attributes.masterMerchantAccount) {
      this.masterMerchantAccount = new MerchantAccount(attributes.masterMerchantAccount);
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.braintree.PayPalAccount"></a>[function <span class="apidocSignatureSpan">braintree.</span>PayPalAccount (attributes)](#apidoc.element.braintree.PayPalAccount)
- description and source-code
```javascript
class PayPalAccount extends AttributeSetter {
  constructor(attributes) {
    super(attributes);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.braintree.Subscription"></a>[function <span class="apidocSignatureSpan">braintree.</span>Subscription ()](#apidoc.element.braintree.Subscription)
- description and source-code
```javascript
class Subscription extends AttributeSetter {
  static initClass() {
    this.Source = {
      Api: 'api',
      ControlPanel: 'control_panel',
      Recurring: 'recurring'
    };

    this.Status = {
      Active: 'Active',
      Canceled: 'Canceled',
      Expired: 'Expired',
      PastDue: 'Past Due',
      Pending: 'Pending',
      All() {
        let all = [];

        for (let key in this) {
          if (!this.hasOwnProperty(key)) {
            continue;
          }
          let value = this[key];

          if (key !== 'All') { all.push(value); }
        }
        return all;
      }
    };
  }

  constructor(attributes) {
    super(attributes);
    this.transactions = attributes.transactions.map((transactionAttributes) => new Transaction(transactionAttributes));
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.braintree.TestingGateway"></a>[function <span class="apidocSignatureSpan">braintree.</span>TestingGateway (gateway)](#apidoc.element.braintree.TestingGateway)
- description and source-code
```javascript
class TestingGateway extends Gateway {
  constructor(gateway) {
    super();
    this.gateway = gateway;
    this.config = this.gateway.config;
  }

  settle(transactionId, callback) {
    return this.settlementOperationWithEnvironmentCheck(transactionId, 'settle', callback);
  }

  settlementPending(transactionId, callback) {
    return this.settlementOperationWithEnvironmentCheck(transactionId, 'settlement_pending', callback);
  }

  settlementConfirm(transactionId, callback) {
    return this.settlementOperationWithEnvironmentCheck(transactionId, 'settlement_confirm', callback);
  }

  settlementDecline(transactionId, callback) {
    return this.settlementOperationWithEnvironmentCheck(transactionId, 'settlement_decline', callback);
  }

  settlementOperationWithEnvironmentCheck(transactionId, operation, callback) {
    if (this.config.environment === Environment.Production) {
      return callback(exceptions.TestOperationPerformedInProductionError('Test operation performed in production'), null); // eslint
-disable-line new-cap
    }

    return this.gateway.http.put(
      '${this.config.baseMerchantPath()}/transactions/${transactionId}/${operation}',
      null,
      callback
    );
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.braintree.Transaction"></a>[function <span class="apidocSignatureSpan">braintree.</span>Transaction ()](#apidoc.element.braintree.Transaction)
- description and source-code
```javascript
class Transaction extends AttributeSetter {
  static initClass() {
    this.CreatedUsing = {
      FullInformation: 'full_information',
      Token: 'token'
    };

    this.EscrowStatus = {
      HoldPending: 'hold_pending',
      Held: 'held',
      ReleasePending: 'release_pending',
      Released: 'released',
      Refunded: 'refunded'
    };

    this.Source = {
      Api: 'api',
      ControlPanel: 'control_panel',
      Recurring: 'recurring'
    };

    this.Type = {
      Credit: 'credit',
      Sale: 'sale',
      All() {
        let all = [];

        for (let key in this) {
          if (!this.hasOwnProperty(key)) {
            continue;
          }
          let value = this[key];

          if (key !== 'All') { all.push(value); }
        }
        return all;
      }
    };

    this.GatewayRejectionReason = {
      ApplicationIncomplete: 'application_incomplete',
      Avs: 'avs',
      Cvv: 'cvv',
      AvsAndCvv: 'avs_and_cvv',
      Duplicate: 'duplicate',
      Fraud: 'fraud',
      ThreeDSecure: 'three_d_secure'
    };

    this.IndustryData = {
      Lodging: 'lodging',
      TravelAndCruise: 'travel_cruise'
    };

    this.Status = {
      AuthorizationExpired: 'authorization_expired',
      Authorizing: 'authorizing',
      Authorized: 'authorized',
      GatewayRejected: 'gateway_rejected',
      Failed: 'failed',
      ProcessorDeclined: 'processor_declined',
      Settled: 'settled',
      Settling: 'settling',
      SettlementConfirmed: 'settlement_confirmed',
      SettlementDeclined: 'settlement_declined',
      SettlementPending: 'settlement_pending',
      SubmittedForSettlement: 'submitted_for_settlement',
      Voided: 'voided',
      All() {
        let all = [];

        for (let key in this) {
          if (!this.hasOwnProperty(key)) {
            continue;
          }
          let value = this[key];

          if (key !== 'All') { all.push(value); }
        }
        return all;
      }
    };
  }

  constructor(attributes) {
    super(attributes);
    this.creditCard = new CreditCard(attributes.creditCard);
    this.paypalAccount = new PayPalAccount(attributes.paypal);
    this.coinbaseAccount = new CoinbaseAccount(attributes.coinbaseAccount);
    this.applePayCard = new ApplePayCard(attributes.applePay);
    this.androidPayCard = new AndroidPayCard(attributes.androidPayCard);
    this.disbursementDetails = new DisbursementDetails(attributes.disbursementDetails);
    if (attributes.disputes != null) { this.disputes = attributes.disputes.map((disputeAttributes) => new Dispute(disputeAttributes
)); }
    if (attributes.facilitatorDetails) { this.facilitatorDetails = new FacilitatorDetails(attributes.facilitatorDetails); }
    if (attributes.riskData) { this.riskData = new RiskData(attributes.riskData); }
    if (attributes.threeDSecureInfo) { this.threeDSecureInfo = new ThreeDSecureInfo(attributes.threeDSecureInfo); }
    if (attributes.usBankAccount) { this.usBankAccount = new UsBankAccount(attributes.usBankAccount); }
  }

  isDisbursed() {
    return this.disbursementDetails.isValid();
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.braintree.ValidationErrorCodes"></a>[function <span class="apidocSignatureSpan">braintree.</span>ValidationErrorCodes ()](#apidoc.element.braintree.ValidationErrorCodes)
- description and source-code
```javascript
class ValidationErrorCodes {
  static initClass() {
    this.Address = {
      CannotBeBlank: '81801',
      CompanyIsInvalid: '91821',
      CompanyIsTooLong: '81802',
      CountryCodeAlpha2IsNotAccepted: '91814',
      CountryCodeAlpha3IsNotAccepted: '91816',
      CountryCodeNumericIsNotAccepted: '91817',
      CountryNameIsNotAccepted: '91803',
      ExtendedAddressIsInvalid: '91823',
      ExtendedAddressIsTooLong: '81804',
      FirstNameIsInvalid: '91819',
      FirstNameIsTooLong: '81805',
      InconsistentCountry: '91815',
      IsInvalid: '91828',
      LastNameIsInvalid: '91820',
      LastNameIsTooLong: '81806',
      LocalityIsInvalid: '91824',
      LocalityIsTooLong: '81807',
      PostalCodeInvalidCharacters: '81813',
      PostalCodeIsInvalid: '91826',
      PostalCodeIsRequired: '81808',
      PostalCodeIsTooLong: '81809',
      RegionIsInvalid: '91825',
      RegionIsTooLong: '81810',
      StateIsInvalidForSellerProtection: '81827',
      StreetAddressIsInvalid: '91822',
      StreetAddressIsRequired: '81811',
      StreetAddressIsTooLong: '81812',
      TooManyAddressesPerCustomer: '91818'
    };

    this.ApplePayCard = {
      ApplePayCardsAreNotAccepted: '83501',
      CustomerIdIsRequiredForVaulting: '83502',
      TokenIsInUse: '93503',
      PaymentMethodNonceConsumed: '93504',
      PaymentMethodNonceUnknown: '93505',
      PaymentMethodNonceLocked: '93506',
      PaymentMethodNonceCardTypeIsNotAccepted: '83518',
      CannotUpdateApplePayCardUsingPaymentMethodNonce: '93507',
      NumberIsRequired: '93508',
      ExpirationMonthIsRequired: '93509',
      ExpirationYearIsRequired: '93510',
      CryptogramIsRequired: '93511',
      DecryptionFailed: '83512',
      Disabled: '93513',
      MerchantNotConfigured: '93514',
      MerchantKeysAlreadyConfigured: '93515',
      MerchantKeysNotConfigured: '93516',
      CertificateInvalid: '93517',
      CertificateMismatch: '93519',
      InvalidToken: '83520',
      PrivateKeyMismatch: '93521',
      KeyMismatchStoringCertificate: '93522'
    };

    this.AuthorizationFingerprint = {
      InvalidCreatedAt: '93204',
      InvalidFormat: '93202',
      InvalidPublicKey: '93205',
      InvalidSignature: '93206',
      MissingFingerprint: '93201',
      OptionsNotAllowedWithoutCustomer: '93207',
      SignatureRevoked: '93203'
    };

    this.ClientToken = {
      CustomerDoesNotExist: '92804',
      FailOnDuplicatePaymentMethodRequiresCustomerId: '92803',
      MakeDefaultRequiresCustomerId: '92801',
      ProxyMerchantDoesNotExist: '92805',
      VerifyCardRequiresCustomerId: '92802',
      MerchantAccountDoesNotExist: '92807',
      UnsupportedVersion: '92806'
    };

    this.CreditCard = {
      BillingAddressConflict: '91701',
      BillingAddressFormatIsInvalid: '91744',
      BillingAddressIdIsInvalid: '91702',
      CannotUpdateCardUsingPaymentMethodNonce: '91735',
      CardholderNameIsTooLong: '81723',
      CreditCardTypeIsNotAccepted: '81703',
      CreditCardTypeIsNotAcceptedBySubscriptionMerchantAccount: '81718',
      CustomerIdIsInvalid: '91705',
      CustomerIdIsRequired: '91704',
      CvvIsInvalid: '81707',
      CvvIsRequired: '81706',
      CvvVerificationFailed: '81736',
      DuplicateCardExists: '81724',
      ExpirationDateConflict: '91708',
      ExpirationDateIsInvalid: '81710',
      ExpirationDateIsRequired: '81709',
      ExpirationDateYearIsInvalid: '81711',
      ExpirationMonthIsInvalid: '81712',
      ExpirationYearIsInvalid: '81713',
      InvalidParamsForCreditCardUpdate: '91745',
      InvalidVenmoSDKPaymentMethodCode: '91727',
      NumberHasInvalidLength: '81716',
      NumberIsInvalid: '81715',
      NumberIsProhibited: '81750',
      NumberIsRequired: '81714',
      NumberLengthIsInvalid: '81716',
      NumberMustBeTestNumber: '81717',
      PaymentMethodConflict: '81725',
      PaymentMethodIsNotACreditCard: '91738',
      PaymentMethodNonceCardTypeIsNotAccepted: '91734',
      PaymentMethodNonceConsumed: '91731',
      PaymentMethodNonceLocked: '91733',
      PaymentMethodNonceUnknown: '91732',
      Post ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.braintree.VenmoAccount"></a>[function <span class="apidocSignatureSpan">braintree.</span>VenmoAccount (attributes)](#apidoc.element.braintree.VenmoAccount)
- description and source-code
```javascript
class VenmoAccount extends AttributeSetter {
  constructor(attributes) {
    super(attributes);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.braintree.WebhookNotification"></a>[function <span class="apidocSignatureSpan">braintree.</span>WebhookNotification ()](#apidoc.element.braintree.WebhookNotification)
- description and source-code
```javascript
class WebhookNotification extends AttributeSetter {
  static initClass() {
    this.Kind = {
      AccountUpdaterDailyReport: 'account_updater_daily_report',
      Check: 'check',
      Disbursement: 'disbursement',
      DisbursementException: 'disbursement_exception',
      DisputeOpened: 'dispute_opened',
      DisputeLost: 'dispute_lost',
      DisputeWon: 'dispute_won',
      PartnerMerchantConnected: 'partner_merchant_connected',
      PartnerMerchantDisconnected: 'partner_merchant_disconnected',
      PartnerMerchantDeclined: 'partner_merchant_declined',
      SubscriptionCanceled: 'subscription_canceled',
      SubscriptionChargedSuccessfully: 'subscription_charged_successfully',
      SubscriptionChargedUnsuccessfully: 'subscription_charged_unsuccessfully',
      SubscriptionExpired: 'subscription_expired',
      SubscriptionTrialEnded: 'subscription_trial_ended',
      SubscriptionWentActive: 'subscription_went_active',
      SubscriptionWentPastDue: 'subscription_went_past_due',
      SubMerchantAccountApproved: 'sub_merchant_account_approved',
      SubMerchantAccountDeclined: 'sub_merchant_account_declined',
      TransactionDisbursed: 'transaction_disbursed',
      TransactionSettled: 'transaction_settled',
      TransactionSettlementDeclined: 'transaction_settlement_declined'
    };
  }

  constructor(attributes) {
    super(attributes);

    let wrapperNode;

    if (attributes.subject.apiErrorResponse != null) {
      wrapperNode = attributes.subject.apiErrorResponse;
    } else {
      wrapperNode = attributes.subject;
    }

    if (wrapperNode.subscription != null) {
      this.subscription = new Subscription(wrapperNode.subscription);
    }

    if (wrapperNode.merchantAccount != null) {
      this.merchantAccount = new MerchantAccount(wrapperNode.merchantAccount);
    }

    if (wrapperNode.disbursement != null) {
      this.disbursement = new Disbursement(wrapperNode.disbursement);
    }

    if (wrapperNode.transaction != null) {
      this.transaction = new Transaction(wrapperNode.transaction);
    }

    if (wrapperNode.partnerMerchant != null) {
      this.partnerMerchant = new PartnerMerchant(wrapperNode.partnerMerchant);
    }

    if (wrapperNode.dispute != null) {
      this.dispute = new Dispute(wrapperNode.dispute);
    }

    if (wrapperNode.accountUpdaterDailyReport != null) {
      this.accountUpdaterDailyReport = new AccountUpdaterDailyReport(wrapperNode.accountUpdaterDailyReport);
    }

    if (wrapperNode.errors != null) {
      this.errors = new ValidationErrorsCollection(wrapperNode.errors);
      this.message = wrapperNode.message;
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.braintree.connect"></a>[function <span class="apidocSignatureSpan">braintree.</span>connect (new Config(config)](#apidoc.element.braintree.connect)
- description and source-code
```javascript
config => new BraintreeGateway(new Config(config))
```
- example usage
```shell
...
* [Documentation](https://developers.braintreepayments.com/node/sdk/server/overview)
* [Bug Tracker](http://github.com/braintree/braintree_node/issues)

## Quick Start
'''javascript
var braintree = require('braintree');

var gateway = braintree.connect({
  environment: braintree.Environment.Sandbox,
  merchantId: 'your_merchant_id',
  publicKey: 'your_public_key',
  privateKey: 'your_private_key'
});

gateway.transaction.sale({
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
