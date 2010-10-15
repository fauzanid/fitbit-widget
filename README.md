# Fitbit widget  

A simple app to help users brows fitbit data on mobile devices or embed it in webpages.

Also a example of how to build mobile sites and apps.

__GETTING STARTED__

* There is no rake task to install gems for you. Look at the requires at the top of fitbit-widget.rb
* Also you can look at the .gems file which installs gems on Heroku
* Unfortunately to really try this code you need a fitbit account
  * set fitbit_email and fitbit_pass to your environment to get tests or the project working
  * you can do this via fitbit_email=my@email.com fitbit_pass=pass ruby fitbit-widget.rb or set them in your .bash_profile
* `rake test`, to run the tests
* `ruby fitbit-widget.rb` to start the sinatra server

## Author
* Dan Mayer (danmayer)

__TODO__
* work on caching all the files/CSS/images
* make it easier to get up and running (rake gems install? )
* log currently logs password, apply a filter to the log to not record passwords.
* support offline online mode on phonegap (currently sort of does with jquery-offline, but doesn't worn on older androids)
* Use progressive updating via jquery opposed to the hardcoded onclick function calls.
* move sinatra simple account to gem and provide plugin mechanism.
  * ie use SinatraSimpleAccount :success => x, :protocall => {} , etc
  * clean up and make all the above options setable
* menu with actual quit option (close option)
* chris hates my fonts bug my design buddy for better design.
* larger clickable links in the UI
* add viewable notice for offline mode
* Real cached assests
* Better shared image solution than local images and full page to site images, same relative path.
* Add arbitrary background tracking using accelerometers and/or GPS, so non fitbit users can have a value.