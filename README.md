# laravel-otp

OTP package for Laravel (Twilio, Fast2SMS, Email drivers). Easy-to-use, pluggable drivers.

## Features
- Send OTP via Twilio, Fast2SMS, Email
- Store hashed OTPs in DB with TTL & verify
- Publishable migrations & config
- Extensible: add custom drivers

## Installation
```bash
composer require zerontech/laravel-otp
php artisan vendor:publish --provider="ZeronTech\LaravelOtp\OtpServiceProvider" --tag="config"
php artisan vendor:publish --provider="ZeronTech\LaravelOtp\OtpServiceProvider" --tag="migrations"
php artisan migrate