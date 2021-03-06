# RSpecHoneycombFormatter

This is a simple RSpec formatter that will send all events to the https://honeycomb.io dataset configured in the environment.
See [honeycombio/beeline-ruby#master lib/honeycomb/configuration.rb](https://github.com/honeycombio/beeline-ruby/blob/master/lib/honeycomb/configuration.rb) for the settings you can use.

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'rspec_honeycomb_formatter'
```

## Usage

Add this line to your .rspec file, or add similar configuration to your RSpec rake task:

```
--require rspec_honeycomb_formatter
--format RSpecHoneycombFormatter
```

Running your spec tests will now send output to honeycomb.


## Development

To install this gem onto your local machine, run `bundle exec rake install`.
To release a new version, update the version number in `version.rb`, and then run `bundle exec rake release`, which will create a git tag for the version, push git commits and tags, and push the `.gem` file to [rubygems.org](https://rubygems.org).

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/puppetlabs/rspec_honeycomb_formatter.
