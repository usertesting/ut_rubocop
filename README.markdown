# UT Rubocop

This is a basic extraction of common UserTesting ruby styles.
For rails focused styles, see [ut_rubocop_rails](https://github.com/usertesting/ut_rubocop_rails)

## Installation

Add the gem to your `Gemfile` in the dev/test group:

You don't need to add `rubocop` itself, this takes care of that.

```ruby
group :test, :development do
  ...
  gem "ut-rubocop", require: false
```

In your `.rubocop.yml` file, add these lines near the top:

```yaml
inherit_gem:
  ut-rubocop:
    - default.yml
```

## Usage

`bundle exec rubocop`

## License

[MIT](LICENSE).

Library created by [UserTesting](https://usertesting.com)

![UserTesting](doc/UserTesting.png)

## Contributing

1. Fork it ( https://github.com/usertesting/ut_rubocop/fork )
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create a new Pull Request
