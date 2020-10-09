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

## Updating Gem

- Increase version number in `lib/ut/style_ruby/version.rb` in your PR.
- After merging to main, tag the current HEAD with the version number chosen: `git tag v0.0.x`
- Build the gem: `gem build .gemspec`
- Push gem to rubygems.org: `gem push ut-rubocop-0.0.x.gem`

The gem is now updated on [rubygems.org](https://rubygems.org/gems/ut-rubocop).

_Note that you will need to be added as a maintainer of the gem to be able to push it._

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
