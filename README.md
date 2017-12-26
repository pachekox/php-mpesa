# M-PESA API Package
[![Build Status](https://travis-ci.org/Kabangi/mpesa.svg?branch=master)](https://travis-ci.org/Kabangi/mpesa)
[![Total Downloads](https://poser.pugx.org/kabangi/mpesa/d/total.svg)](https://packagist.org/packages/smodav/mpesa)
[![Latest Stable Version](https://poser.pugx.org/kabangi/mpesa/v/stable.svg)](https://packagist.org/packages/kabangi/mpesa)
[![Latest Unstable Version](https://poser.pugx.org/kabangi/mpesa/v/unstable.svg)](https://packagist.org/packages/kabangi/mpesa)
[![License](https://poser.pugx.org/kabangi/mpesa/license.svg)](https://packagist.org/packages/kabangi/mpesa)

This is a PHP package with first class support to laravel for the Safaricom's M-Pesa REST API dubbed DARAJA API.  

It implements all the exposed endpoints by Safaricom as listed below:-

### 1. [Lipa na M-Pesa Online Payment](https://developer.safaricom.co.ke/docs#lipa-na-m-pesa-online-payment)
#### &nbsp; &nbsp; What it is?
The Lipa na M-Pesa Online Payment endpoint(STK push) allows you to request payment from your users/clients. With this endpoint all the user is required to do is input their M-PESA pin to a prompt to send a payment to you. 
#### &nbsp; &nbsp; How to implement it?
[Read docs here](https://github.com/Kabangi/mpesa/edit/master/docs/LipaNaMpesaOnline.md).

### 2. [Lipa na M-Pesa Online Query Request](https://developer.safaricom.co.ke/docs#lipa-na-m-pesa-online-query-request)
#### &nbsp; &nbsp; What it is?
When you request payment from your users/clients via Lipa na M-Pesa Online endpoint above you might want to know the status of that request. This endpoint facilitates that. It allows you to query the status of any STK push on demand. 
#### &nbsp; &nbsp; How to implement it?
Read docs here.

### 3. [C2B](https://developer.safaricom.co.ke/docs#c2b-api)
#### &nbsp; &nbsp; What it is?
This endpoint enables developers to receive real time notifications when a client makes a payments to a merchant's Till number or Paybill number. It assumes the payment are made via the SIM card toolkit and as a developer you need to know when that payment hits the merchants till/paybill number for reconciliation and accounting purposes.
#### &nbsp; &nbsp; How to implement it?
Read docs here.

### 4. [B2C](https://developer.safaricom.co.ke/docs#b2c-api)
#### &nbsp; &nbsp; What it is?
This endpoints enables merchants to pay their customers from they paybill account. Some of the use cases are but not limited to paying salaries, paying promotions to customers etc.
#### &nbsp; &nbsp; How to implement it?
Read docs here.

### 5. [B2B](https://developer.safaricom.co.ke/docs#b2b-api)
#### &nbsp; &nbsp; What it is?
This endpoint allows merchants to transfer funds from business to business accounts. 
#### &nbsp; &nbsp; How to implement it?
Read docs here.

### 6. [Transaction Status](https://developer.safaricom.co.ke/docs#transaction-status)
#### &nbsp; &nbsp; What it is?
This endpoint enables developers to initiate status check of a B2B, B2C and C2B transactions. It really comes in handy where one party in a transactions fails/claims not to have received an acknowledgment for a transaction.
#### &nbsp; &nbsp; How to implement it?
Read docs here.

### 7. [Reverse API](https://developer.safaricom.co.ke/docs#reversal)
#### &nbsp; &nbsp; What it is?
This endpoint enables merchants to reverse a B2B, B2C or C2B transaction. It allows automation of reversal of erronous payment to a merchant's paybill/till number or payments to goods never delivered.
#### &nbsp; &nbsp; How to implement it?
Read docs here.

### 8. [Account Balance](https://developer.safaricom.co.ke/docs#account-balance-api)
#### &nbsp; &nbsp; What it is?
This endpoint enables merchants to query their Till/Paybill numbers account balance on demand.
#### &nbsp; &nbsp; How to implement it?
Read docs here.

## Installation

This project is distributed via composer package manager and should be installed as one of your project's dependencies:

```
composer require kabangi/mpesa
```

## Configuration
When using vanilla PHP, modify your `composer.json` file to include:

```json
  "scripts": {
        "post-update-cmd": [
            "Kabangi\\Mpesa\\Support\\Installer::install"
        ]
  },
```
This script will copy the default configuration file to a config folder in the root directory of your project.
Now proceed to require the package.

## Usage

List all the endpoints here and link to the specific endpoint page

## Inspiration

## Contributors

## Support

## License

The M-Pesa Package is open-sourced software licensed under the [MIT license](http://opensource.org/licenses/MIT).
