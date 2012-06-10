# RailsCasts Episode #48: Console Tricks (revised)

http://railscasts.com/episodes/48-console-tricks (revised)

Requires Ruby 1.9.2 or higher.


### Commands used in rails console

```ruby
app.products_path
app.get _
app.class
app.cookies
app.response.headers
pp _; nil
puts app.response.body
app.assigns(:products).size

helper.number_to_currency(123.456)
helper.controller = controller
controller.params = {foo: "bar"}
helper.params

reload!
Product.first.to_param

Product.count
ActiveRecord::Base.logger.level = 1

y Product.first

helper.mate(:number_to_currency)

require 'hirb'
Hirb.enable
Product.limit(5)

require 'awesome_print'
ap Product.first.attributes

require 'clipboard'
Clipboard.copy 'foobar'
Clipboard.paste

require 'methodfinder'
"abc".find_method("ABC")

require 'fancy_irb'
FancyIrb.start
3 + 5

require 'wirb'
Wirb.start
3 + 5
```
