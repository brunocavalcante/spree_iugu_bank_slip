Spree Iugu BankSlip [![Build Status](https://travis-ci.org/zaeznet/spree_iugu_bank_slip.svg?branch=master)](https://travis-ci.org/zaeznet/spree_iugu_bank_slip)
=================

Add to Spree Commerce the payment by [Iugu](http://c.iugu.com/) Bank Slip.

Installation
------------

Add spree_iugu_bank_slip to your Gemfile:

```ruby
gem 'spree_iugu_bank_slip'
```

Bundle your dependencies and run the installation generator:

```shell
bundle
bundle exec rails g spree_iugu_bank_slip:install
```

Settings
------------

To configure the settings, you can go to admin/bank_slip_settings page, or in an initialize file you can modify the settings like that:

```ruby
Spree::BankSlipConfig[:iugu_api_token] = 'ABC1234'
```

Testing
-------

First bundle your dependencies, then run `rake`. `rake` will default to building the dummy app if it does not exist, then it will run specs. The dummy app can be regenerated by using `rake test_app`.

```shell
bundle
bundle exec rake
```

When testing your applications integration with this extension you may use it's factories.
Simply add this require statement to your spec_helper:

```ruby
require 'spree_iugu_bank_slip/factories'
```

Copyright (c) 2016 [Zaez Comunicação Digital], released under the New BSD License
