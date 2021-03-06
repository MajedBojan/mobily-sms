# Mobily::Sms

mobily-sms gem used to integrate with [Mobilyws](http://mobily.ws/sms/index.php) api's. mobilyws offers a SMS Gateway service "SMS API", that allows you easily connect Send-SMS service with your applications, websites, or any kind of systems that you may have

This gem will make your integration with [Mobilyws](http://mobily.ws/sms/index.php) easier, In order to use mobily.ws API, you should have a Mobily.ws account from [Mobilyws](http://mobily.ws/sms/index.php).

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'mobily-sms'
```

And then execute:

```
$ bundle
```

Or install it yourself as:

```
$ gem install mobily-sms
```

## Usage

After installing the gem create file in `config/initializers/mobily_credentials.rb` and call it `mobily_credentials.rb` then copy these lines

```
$smshost = `TODO: add your sender name from mobily.we`

USERNAME = 'TODO: add your username from mobily.we'
PASSWORD = `TODO: add your password from mobily.we`
$mobily_credentials = MobilyApiAuth.new( USERNAME, PASSWORD)
```

Here we go, now we can send our message

```
Sms.send('967xxxxxxxxx', 'Hey, Mobily.ws service integrated successfully')
```

## Development

After checking out the repo, run `bin/setup` to install dependencies. Then, run `rake spec` to run the tests. You can also run `bin/console` for an interactive prompt that will allow you to experiment.

To install this gem onto your local machine, run `bundle exec rake install`. To release a new version, update the version number in `version.rb`, and then run `bundle exec rake release`, which will create a git tag for the version, push git commits and tags, and push the `.gem` file to [rubygems.org](https://rubygems.org).

## Contributing

Bug reports and pull requests are welcome on GitHub at <https://github.com/majedbojan/mobily-sms>. This project is intended to be a safe, welcoming space for collaboration, and contributors are expected to adhere to the [Contributor Covenant](http://contributor-covenant.org) code of conduct.

## License

The gem is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).

## Code of Conduct

Everyone interacting in the Mobily::Sms project's codebases, issue trackers, chat rooms and mailing lists is expected to follow the [code of conduct](https://github.com/[USERNAME]/mobily-sms/blob/master/CODE_OF_CONDUCT.md).
