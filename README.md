# AllowNumeric

This gem provides easy way to restrict numeric input to input fields using jquery and integrates with Rails asset pipeline for easy of use.


## Installation

Add this line to your application's Gemfile:

```ruby
gem 'allow_numeric'
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install allow_numeric

## Usage

### Add following line to "app/assets/javascripts/application.js"
```
//= require allow_numeric
```
and restart rails server.

## Add ```data-numeric="true"``` to field for which you want to allow numeric input only.

##### For example:

---
```
<%= form_for @person do |f| %>
  ..
  ..
  <%= f.label :phone %>:
  <%= f.text_field :phone, data: { numeric: true } %><br />

  <%= f.submit %>
<% end %>
```


## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/abhikanojia/allow_numeric.

## License

The gem is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).

## Code of Conduct

Everyone interacting in the AllowNumeric project’s codebases, issue trackers, chat rooms and mailing lists is expected to follow the [code of conduct](https://github.com/[USERNAME]/allow_numeric/blob/master/CODE_OF_CONDUCT.md).
