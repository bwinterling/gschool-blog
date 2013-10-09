---
title: Eloquent Ruby
date: 2013-10-08 10:14 UTC
tags: Eloquent, Ruby
---


![Brian Winterling](http://www.gravatar.com/avatar/d6cf7193827cd231b16b02884a459046.png "Brian")

Eloquent Ruby (Russ Olsen) does describy itself fairly well.  Well written, easy to digest, great code samples.  I'd suggest giving it a spin.

gSchool has certainly been preaching these concepts, so a few of the chapters only served as reinforcement.  Listed below are a few things that stood out to me (many of which are quoted straight from the text).  Enjoy.

**Ch 2 - Choose the Right Control Structure**
**\>** You can set a variable to the result of a case statement.  Not sure why I didn't realise this, because Ruby is so flexible.  I guess case statements always felt like logic and not an expression, but I would be wrong.
**\>** When using Boolean logic, just remember that 0 is not false, and that both nil and false are false.  Be careful with that nil == false and how you write your logic.
**\>** Don't use ||= to initialize things to Booleans due to the nil/false confusion.

**Ch 3 - Take Advantage of Ruby's Smart Collections**
**\>** When passing variables to a method, use the \* symbol (splat) in front of the variable to indicate *any number* of arguments instead of one argument.
**\>** The inject method passes the results back into the block.
**\>** *Beware the bang (!).*  And remember, even though most methods that modify the collection have a !, there are a few that don't.  *Push, pop, delete and shift would be a few examples of that.*
**\>** Set is basically an unordered array that removes duplicates.

**Ch 4 - Take Advantage of Ruby's Smart Strings**
**\>** Shortcut for writing strings - %q or %Q partnered with any enclosure.  %q is like ' '.  %Q is like " ".  *For example, %q(Have you read "Eloquent Ruby"?)*.
**\>** Only double quotes can accept string interpolation.

**Ch 5 - Find the Right String with Regular Expressions**
**\>** The regular expression . will match any single-character string including r and % and ~.
**\>** \* matches zero or more of the character that preceded it, hence .\* will match zero or more of any character.
**\>** You use the =~ operator to test whether a regular expression matches a string, and returns the index value of where the match occured, or nil if no match.
**\>** Turn case sensitivity off by add i to your expression.
**\>** To search through multiline text, add m to the expression.

**Ch 6 - Use Symbols to Stand for Something**
**\>** This chapter can be summed up as simply - use symbols when you simply want an intelligible thing that stands for something in your code.  Use strings for data that you wish to process or manipulate (truncate, uppercase, concatenate, etc.).

**Ch 7 - Treat Everything Like and Object**
**\>** Classes basically provide two things:  containers for methods and factories for making instances.
**\>** Ruby treats *self* as a sort of default object.  When you call a method without an explicit object reference, Ruby assumes that you meant to call the method on self.
**\>** If you don't specify a Superclass when defining an object, your new object automatically becomes a subclass of Object.
**\>** The Object.eval(string) takes a string and executes it as if it were Ruby code.
**\>** You cannot call a private method with an explicit object reference (unless you use the send method!).

**Ch 8 - Embrace Dynamic Typing**
**\>** A couple quotes sum up this chapter:
**\>** "Writing a tricky bit of code is like that old circus act where the performer keeps an improbably large number of plates spinning atop vertical sticks, except that here it’s the details of your problem that are spinning and it’s all happening in your head. *When you are coding, anything that reduces the number of revolving mental plates is a win*."
**\>** "The Ruby answer to [most] kinds of bugs is to write automated tests, lots and lots of automated tests."
**\>** "Keep in mind that Ruby classes don’t need to be related by inheritance to share a common interface; they only need to support the same methods. Don’t obscure your code with pointless checks to see whether this really is an instance of that. Do take advantage of the terseness provided by dynamic typing to write code that simply gets the job done with as little fuss as possible — but also keep in mind that someone (possibly you!) will need to read and understand the code in the future.
**Above all, write tests. . . .**"

**Ch 9 - Write Specs!**
**\>** "If you want to know that your code works, you need to test it. You need to test it early, you need to test it often, and you certainly need to test it whenever you change it."
**\>** This chapter reviews rspec and unit test/mini test.  Read again for a review.  Also look for gems that may extend the capabilities of both.  Mocking data and stubbing are possible in both.  There is also a gem to make minitest read more like rspec.
**\>** "The take-away here is that you are not finished until you have both the software and the tests or specs to go with it. Write the tests first, or second, or third. But write the darned tests."

**Ch 10 - Construct Your Classes from Short, Focused Methods**
**\>** "In Ruby, the cost of defining a new method is very low: just an additional def and an extra end. Since defining a new Ruby method adds very little noise to your code, in Ruby you can get the full composed method bang for a very modest code overhead buck."
**\>** You methods should be compact but must also do *something*.

**Ch 11 - Define Operators Respectfully**
**\>** There are many dangers with redefining standard methods in a class, but this quote sums up the general concept:
**\>** "So when should you define operators for your classes and when should you just stick to ordinary methods? Like most software engineering questions, the answer to this one is a resounding “It depends.” Mainly it depends on the kind of object you are defin- ing and the specific operations it supports. The easiest case is where you find yourself building a class that has some natural, intuitive operator definitions. Envy the authors of the Ruby Matrix and Vector classes: The answer to the question of whether to have a + operator—and what that operator should do—is as close as the nearest linear algebra textbook. Similarly, the built-in Set class very logically maps the boolean | and & operators to the union and intersection operations. If you find yourself in a similar situation—you are building a class that has a natural, well-understood meaning for the operators—then count your- self lucky and start coding."
**\>** "Assigning arbitrary, far-fetched meanings to the common operators is one thing that gives programmer-defined operators a bad name. Remember, the goal is clear and concise code."

**Ch 12 - Create Classes That Understand Equality**
**\>** "Ruby’s Object class defines no less than four equality methods. There is eql? and equal? as well as == (that’s two equal signs), not to mention === (that’s three equal signs). For a language that prides itself on simplicity and conciseness, that’s an awful lot of ways of saying nearly the same thing. Nearly, but not exactly the same."
**\>** Ruby uses .equal? to test if they are identically the same object.  Basically the same as ==.
**\>** Classes treat the === method as kind_of?

**Ch 13 - Get the behavior You Need with Singleton and Class Methods**
**\>** 

