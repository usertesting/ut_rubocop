# UT Rubocop

## Installation

Add this line to your application's Gemfile:

```ruby
gem "ut-rubocop"
```

And then execute:

```ruby
$ bundle install
```

## Usage

In your `.rubocop.yml` file, add these lines near the top:

```yaml
inherit_gem:
  ut-rubocop:
    - default.yml
```

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
