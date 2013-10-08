---
title: Eloquent Ruby
date: 2013-10-04 15:14 UTC
tags: Eloquent, Ruby
---


![Brian Winterling](http://www.gravatar.com/avatar/d6cf7193827cd231b16b02884a459046.png "Brian")

Eloquent Ruby does describy itself fairly well.  Well written, easy to digest, great code samples.  I'd suggest giving it a spin.

gSchool has certainly been preaching these concepts, so a few of the chapters only served as reinforcement.  Listed below are a few things that stood out to me.  Enjoy.

**Ch 2**
> You can set a variable to the result of a case statement.  Not sure why I didn't realise this, because Ruby is so flexible.  I guess case statements always felt like logic and not an expression, but I would be wrong.
> When using Boolean logic, just remember that 0 is not false, and that both nil and false are false.  Be careful with that nil == false and how you write your logic.
> Don't use ||= to initialize things to Booleans due to the nil/false confusion.

**Ch 3**
> When passing variables to a method, use the \* symbol (splat) in front of the variable to indicate *any number* of arguments instead of one argument.
> The inject method passes the results back into the block.
> *Beware the bang (!).*  And remember, even though most methods that modify the collection have a !, there are a few that don't.  *Push, pop, delete and shift would be a few examples of that.*
> Set is basically an unordered array that removes duplicates.

**Ch 4**
> Shortcut for writing strings - %q or %Q partnered with any enclosure.  %q is like ' '.  %Q is like " ".  *For example, %q(Have you read "Eloquent Ruby"?)*.
> Only double quotes can accept string interpolation.


