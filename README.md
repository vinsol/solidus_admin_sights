SolidusAdminInsights
==============

Dashboard for querying and viewing you solidus store's metrics. Use SolidusEventTracker to capture the metrics

Installation
------------

Ensure [SolidusEventTracker](https://github.com/vinsol/solidus_events_tracker) is installed.


Add solidus_admin_insights to your Gemfile:

```ruby
gem 'solidus_admin_insights', github: 'vinsol/solidus_admin_insights'
```

Bundle your dependencies and run the installation generator:

```shell
bundle
bundle exec rails g solidus_admin_insights:install
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
require 'solidus_admin_insights/factories'
```

Credits
-------

[![vinsol.com: Ruby on Rails, iOS and Android developers](http://vinsol.com/vin_logo.png "Ruby on Rails, iOS and Android developers")](http://vinsol.com)

Copyright (c) 2016 [vinsol.com](http://vinsol.com "Ruby on Rails, iOS and Android developers"), released under the New MIT License
