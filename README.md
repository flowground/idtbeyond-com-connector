# ![LOGO](logo.png) Active Documentation for /v1 **flow**ground Connector

## Description

A generated **flow**ground connector for the Active Documentation for /v1 API (version 1.1.7).

Generated from: https://api.apis.guru/v2/specs/idtbeyond.com/1.1.7/swagger.json<br/>
Generated at: 2019-06-06T16:12:23+03:00

## API Description

Our active docs provide the ability to test out your account and to see the responses to your queries. The services are RESTful, and are accessed using standard HTTP methods over a secure HTTPS channel. Requests and responses are currently sent in JSON format, and have a base URL of /v1.

## Authorization

This API does not require authorization.

## Actions

### Account balance

> Returns a JSON of the account balance.

*Tags:* `account`

#### Input Parameters
* `x-idt-beyond-app-id` - _required_ - Application ID you would like to use
* `x-idt-beyond-app-key` - _required_ - Application KEY you would like to use

### List of account charges in JSON

> Returns charges by date range.

*Tags:* `charges`

#### Input Parameters
* `x-idt-beyond-app-id` - _required_ - Application ID you would like to use
* `x-idt-beyond-app-key` - _required_ - Application KEY you would like to use
* `date_from` - _required_ - The beginning date of the search IN YYYY-MM-DD format (America/New_York timezone). '2016-01-28'
* `date_to` - _required_ - The ending date of the search IN YYYY-MM-DD format (America/New_York timezone). '2016-01-28'

### List of account charges in CSV

> Returns charges by date range in CSV.

*Tags:* `charges`

#### Input Parameters
* `x-idt-beyond-app-id` - _required_ - Application ID you would like to use
* `x-idt-beyond-app-key` - _required_ - Application KEY you would like to use
* `date_from` - _required_ - The beginning date of the search IN YYYY-MM-DD format (America/New_York timezone). '2016-01-28'
* `date_to` - _required_ - The ending date of the search IN YYYY-MM-DD format (America/New_York timezone). '2016-01-28'

### Mobile number validation

> Checks to verify if the phone number is valid for the country supplied.

*Tags:* `utilities`

#### Input Parameters
* `x-idt-beyond-app-id` - _required_ - Application ID you would like to use
* `x-idt-beyond-app-key` - _required_ - Application KEY you would like to use
* `country_code` - _required_ - 2-digit code of the country in ISO 3166 format. 'BR'
* `mobile_number` - _required_ - The mobile number you would like to validate. '5521983115555'

### Current promotions

> Returns a JSON of the current promotions.

*Tags:* `utilities`

#### Input Parameters
* `x-idt-beyond-app-id` - _required_ - Application ID you would like to use
* `x-idt-beyond-app-key` - _required_ - Application KEY you would like to use

### Get a list of products in JSON format

> Returns a JSON list of products, ranges, and their commissions percentages.

*Tags:* `products`

#### Input Parameters
* `x-idt-beyond-app-id` - _required_ - Application ID you would like to use
* `x-idt-beyond-app-key` - _required_ - Application KEY you would like to use

### Get a list of products in CSV format

> Returns a CSV of products, ranges, and their commissions percentages.

*Tags:* `products`

#### Input Parameters
* `x-idt-beyond-app-id` - _required_ - Application ID you would like to use
* `x-idt-beyond-app-key` - _required_ - Application KEY you would like to use

### Get the estimated Local Value of a product

> Returns a CSV of products, ranges, and their commissions percentages.

*Tags:* `products`

#### Input Parameters
* `x-idt-beyond-app-id` - _required_ - Application ID you would like to use
* `x-idt-beyond-app-key` - _required_ - Application KEY you would like to use
* `country_code` - _required_ - 2-digit code of the country in ISO 3166 format. 'GT'
* `carrier_code` - _required_ - Name of the mobile carrier. 'Claro'
* `amount` - _required_ - This is the amount, in cents, of the product you are purchasing. '500' = $5.00
* `currency_code` - _required_ - The currency code (ISO 4217) on the product you are querying. 'USD'

### Topup a mobile phone

> Submits an IATU transaction request.

*Tags:* `topups`

#### Input Parameters
* `x-idt-beyond-app-id` - _required_ - Application ID you would like to use
* `x-idt-beyond-app-key` - _required_ - Application KEY you would like to use

### Search topups transactions

> Search topups transactions, by date, with client_transaction_id or to_service_number. Use 'client_transaction_id' to search by transaction number, or 'to_service_number' to get transaction status.

*Tags:* `topups`

#### Input Parameters
* `x-idt-beyond-app-id` - _required_ - Application ID you would like to use
* `x-idt-beyond-app-key` - _required_ - Application KEY you would like to use

### List of account topups in JSON

> Returns topups by date range.

*Tags:* `topups`

#### Input Parameters
* `x-idt-beyond-app-id` - _required_ - Application ID you would like to use
* `x-idt-beyond-app-key` - _required_ - Application KEY you would like to use
* `date_from` - _required_ - The beginning date of the search IN YYYY-MM-DD format (America/New_York timezone). '2016-01-28'
* `date_to` - _required_ - The ending date of the search IN YYYY-MM-DD format (America/New_York timezone). '2016-01-28'

### List of account topups in CSV

> Returns topups by date range in CSV.

*Tags:* `topups`

#### Input Parameters
* `x-idt-beyond-app-id` - _required_ - Application ID you would like to use
* `x-idt-beyond-app-key` - _required_ - Application KEY you would like to use
* `date_from` - _required_ - The beginning date of the search IN YYYY-MM-DD format (America/New_York timezone). '2016-01-28'
* `date_to` - _required_ - The ending date of the search IN YYYY-MM-DD format (America/New_York timezone). '2016-01-28'

### Summary of account topups in JSON

> Returns topups totals by date range.

*Tags:* `topups`

#### Input Parameters
* `x-idt-beyond-app-id` - _required_ - Application ID you would like to use
* `x-idt-beyond-app-key` - _required_ - Application KEY you would like to use
* `date_from` - _required_ - The beginning date of the search IN YYYY-MM-DD format (America/New_York timezone). '2016-01-28'
* `date_to` - _required_ - The ending date of the search IN YYYY-MM-DD format (America/New_York timezone). '2016-01-28'

### Reversal of a Topup

> Occasionally, a carrier will not be able to successfully complete a topup request. In this case, we will attempt to automatically reverse the transaction for you, and return the money into your account. In the case when this is not possible, you may need to request a reverse on the transaction that has a status of 'transaction_status' 'notredeemed'.

*Tags:* `topups`

#### Input Parameters
* `x-idt-beyond-app-id` - _required_ - Application ID you would like to use
* `x-idt-beyond-app-key` - _required_ - Application KEY you would like to use

### Status check

> Returns a JSON of the API status.

*Tags:* `utilities`

#### Input Parameters
* `x-idt-beyond-app-id` - _required_ - Application ID you would like to use
* `x-idt-beyond-app-key` - _required_ - Application KEY you would like to use

## License

**flow**ground :- Telekom iPaaS / idtbeyond-com-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
