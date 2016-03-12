# special-couscous

Here we have an example repository which will attempt to have integrated issues between github and trello.

We will use the help listed on http://neverstopbuilding.com/integrating-github-with-trello-with-heroku to get started.
We will tell the posthook to deliver everything. So far my attempts have generated errors in the heroku log of 
TypeError - no implicit conversion of nil into String:

See http://stackoverflow.com/questions/19643153/error-to-install-nokogiri-on-osx-10-9-maverick for more help.

This seems to be an error with rspec, which may or may not be a really old thing that has gone through a few iterations and is now something else. I'm now trying ifttt recipes from ifttt.com. Hmm, it looks like only one of the actions that I'm hoping for is possible through there. (See list below, ifttt recipes handle case (A)


Updated to use explicit versions of ruby, looking promising.

A) If "add a new trello card to specific list" then "start an issue on a specific github repository"

B) If "a new commit github commit mentions a trello card" then "start a new trello card"

C) If "an issue is closed" then "move a trello card"

D) If "a trello card is moved" then "close an issue"


---- Moving to a python based hook because I can read python much better than ruby.
---- Huzzah, a response from the server was received! It didn't do anything to the trello board, but at least I have something to work with now.
