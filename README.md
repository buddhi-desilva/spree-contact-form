Spree Contact Form Extension
=========

An spree extension for contact forms with reCAPTCHA

Installation
============

1) add the gem to your `Gemfile`:

`gem 'spree_contact_form'`

2) run bundler:

`bundle install`

3) install it:

`rails generate spree_contact_form:install`

3) migrate your database:

`rake db:migrate`

4) Configure reCAPTCHA

You may use the block style configuration. The following code could be placed
into a +config/initializers/recaptcha.rb+ when used in a Rails project.

`Recaptcha.configure do |config|
  config.public_key  = '6Lc6BAAAAAAAAChqRbQZcn_yyyyyyyyyyyyyyyyy'
  config.private_key = '6Lc6BAAAAAAAAKN3DRm6VA_xxxxxxxxxxxxxxxxx'
  config.proxy = 'http://myproxy.com.au:8080'
end`

check: https://github.com/ambethia/recaptcha/ and http://www.google.com/recaptcha for more information on configuring reCAPTCHA


Viewing Contact Form
======================

`http://yourdomain.tld/contact`
