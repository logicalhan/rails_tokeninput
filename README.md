# Rails Tokeninput

**Rails Tokeninput** is a small, lightweight gem which helps to automate installing of the jquery tokeninput plugin, including the standard included stylesheets.

# JqueryTokeninput Version

The current release of this gem is using **Version 1.6.0**

# Included Javascripts/Stylesheets

	jquery.tokeninput.js

	token-input-facebook.css
	token-input-mac.css
	token-input.css

### Installation

This gem should work out of the box. All you have to do is add the gem to your Gemfile: 

	gem 'rails_tokeninput'

Then bundle install or update (depending on if you want to upgrade an older version of this gem).
	
	bundle install
	bundle update
	
In your assets/javascripts/application.js, you will need to add d3 to your manifest:
	
	//= require jquery
	.
	.
	//= require jquery.tokeninput
	
In your assets/stylesheets/application.css, you can add the stylesheets you want by including them in your css manifest:

	*= require_self
	.
	.
	*= require token-input-facebook
	..etc.
