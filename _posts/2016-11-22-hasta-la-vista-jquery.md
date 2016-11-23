---
title:        "Hasta la vista, jQuery"
# jekyll-seo-tag
description:  "jQuery has been removed from Rails"
author:       "guilleiguaran"
---

Some of you might remember how excited we were back in 2010 when Rails 3
introduced the option to use JavaScript libraries as alternative to
Prototype/Scriptaculus (someone else is feeling old?) like Mootools
(do you remember Mootools, right?) and jQuery, some others might remember how "hacky" was
[using jQuery with Rails helpers in Rails 2.3](https://github.com/aaronchi/jrails/blob/master/lib/jrails.rb)),
and others might remember also how excited we were with the
introduction of Unobstrusive JavaScript (we had AJAX without writing one
single line of code!!)

Back in 2010 (and before) avoiding writing vanilla JavaScript and using
frameworks for DOM manipulation, AJAX, events, etc was totally reasonable.
Today the panorama is totally different: do you event listeners? AJAX?
bind? You're totally covered by ES5 (and hey ES7 is the last thing
nowadays!!), do you need `$(document).ready?`
[DOMContentLoaded](https://developer.mozilla.org/en-US/docs/Web/Events/DOMContentLoaded)
from HTML5 is your new best friend.

Maybe there are plenty of other reasons for using jQuery in many
applications, that's totally fine but many would agree that it is
not a standard or default for the new applications today and that's why
we have decided to [move it out from default Rails stack](https://github.com/rails/rails/pull/27113)
to RoR Retirement Home (remember [TRL Retirement Home](http://atrl.net/trlarchive/?s=halloffame)?).

UJS is now supported using [rails-ujs](https://github.com/rails/rails-ujs) library
(that doesn't use any framework underhood) created by [Dangyi Liu](https://github.com/liudangyi)
as part of Google Summer of Code and you can still use jQuery in your
new apps with the `-j` option (e.g `rails new blog -j jquery`)... or (protip!) you can
use that option to get React instead (`rails new instagram -j react`) ;-).

Too much nostalgia for a day, hasta la vista, jQuery. (do you remember that old movie? right?)