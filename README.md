# Debugging Drill: Using A REPL

##Learning Competencies

##Summary

 The [Interactive Ruby Shell](http://en.wikipedia.org/wiki/Interactive_Ruby_Shell) is a command-line interface where you can execute Ruby code. It has access to the full Ruby language, so you can utilize all of the features from within a console.

IRB is Ruby's [REPL](http://en.wikipedia.org/wiki/Read%E2%80%93eval%E2%80%93print_loop), or read-eval-print-loop. REPL is pronounced like "reh-pull". Most languages have a REPL and they work roughly the same way:

<dl>
  <dt>Read</dt>
  <dd>A user is prompted to input Ruby expression like <code>5 + 4</code> or <code>"apples".reverse</code>.</dd>
  <dt>Evaluate</dt>
  <dd>After the user hits enter, the REPL evaluates the expression.</dd>
  <dt>Print</dt>
  <dd>The REPL prints out what the expression evaluates to, that is, <code>5 + 4</code> evaluates to <code>9</code>.</dd>
  <dt>Loop</dt>
  <dd>We return to the first step, where the user is prompted to input a Ruby expression</dd>
</dl>

IRB is a great place to experiment and play with Ruby. Think of it as a sandbox: you can try anything, and there are no consequences. You are not saving your code to a file or posting it to GitHub, so you are only limited by your own imagination and willingness to explore.

To load IRB, simply open your Terminal and run the command `irb`. You should see your command prompt change to something like this: `1.9.3p194 :001 > `. Now you can write Ruby code that will execute immediately.

*Note*: the number on the left - `1.9.3p194` indicates the current version of Ruby; it may be different on your machine.

## Learning Goals
* Using IRB.
* Research a new tool and understand when it is useful.
* Testing code without attachment.

## Objectives

### Define a method

In IRB, define a method `say_hi` that takes a person's name as an argument and returns a simple greeting.

For example, if you use the name "Shereef", `say_hi` would return `"Hi, Shereef"`. Then call the method with with your name as the argument.

### Assign variables

Assign values to a few different variables. Use integers, strings, symbols, hashes, arrays - anything you want.

Things to try:

- Using destructive methods
- Comparing `object_id`
- Using `#inspect`

### Include a module

Type `Math.sqrt(1282)`. Or `Time.now`. Or `Array.new(10, 'bee')`. You can access all the built-in modules and classes like this. Isn't that special?

Include the `Math` module in your current IRB environment by typing:

```text
:001 > include Math
```

This loads the methods from the `Math` module into the global object. Now if you type `sqrt 64` it should return `8`.

###Done!

Copy the IRB history that you've created and paste it in your gist!

##Releases
###Release 0

##Optimize Your Learning

##Resources