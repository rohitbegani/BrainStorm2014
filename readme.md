BrainStorm-Quiz-Website-Engine
==============================
BrainStorm is a quiz/treasure hunt website engine. It is based on Ruby on Rails and maybe used by anyone to host their own online quiz/treasure hunt event.
The first instance of this Quiz-Website-Engine was used in May 2014 and maybe seen at bstorm2014.com
It is currently undergoing rigorous testing and all the test cases will be uploaded on Github soon.

How to Use
----------
*Fork the project and clone it
*Run `bundle Install`
*Then run these commands

```ruby
rake db:migrate \\migrate the databases
rake db:create  \\Create environment
```

Setting up and Running the game
-------------------------------
Initialize the game
-------------------
```ruby
rake game:initialize
```

Launch the game
---------------
```ruby
rake game:launch
```

Stop the game
-------------
```ruby
rake game:kill
```

Features
--------
*Seperate admin panel for adding/editing/removing questions
*Connectivity with google analytics
*A fully connected leaderboard
*Optimized for hosting on Heroku
*Powerful regex for answer checking i.e. spaces, case, indentation and punctuation don't matter. For example; if the answer is Ruby Ninja, then rubyninja, RubyNinja, ruby ninja and even Ruby Ninja! all are correct answers.

Google Analytics
----------------

Google Analytics has been connected using the google-analytics-rails gem by bgarret.

To use google analytics go to:

`config\environments\production.rb`

After that replace # with your tracker code

`GA.tracker = "UA-########-##"

That's it!