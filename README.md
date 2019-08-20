# SpreeFixedAmountDiscount

Introduction goes here.

## Installation

1. Add this extension to your Gemfile with this line:
  ```ruby
  gem 'spree_fixed_amount_discount', github: 'matthewkennedy/spree_fixed_amount_discount'
  ```

2. Install the gem using Bundler:
  ```ruby
  bundle install
  ```

3. Restart your server

  If your server was running, restart it so that it can find the assets properly.

## Using

Under the Promotion Actions panel select Create per-line-item adjustment and click Add. In the drop-down menu you should see **Fixed Amount (Items total)**, select this, click update and then enter a fixed amount and currency that you want to deduct from the order.

You should now have a whole order style discount that takes into account each line items tax.

**NOTE:** Please be aware that this promotion will not be calculated correctly if you set Product Based Rules.

## Testing

First bundle your dependencies, then run `rake`. `rake` will default to building the dummy app if it does not exist, then it will run specs. The dummy app can be regenerated by using `rake test_app`.

```shell
bundle
bundle exec rake
```

When testing your applications integration with this extension you may use it's factories.
Simply add this require statement to your spec_helper:

```ruby
require 'spree_fixed_amount_discount/factories'
```


## Contributing

If you'd like to contribute, please take a look at the
[instructions](CONTRIBUTING.md) for installing dependencies and crafting a good
pull request.

Copyright (c) 2019 [name of extension creator], released under the New BSD License
