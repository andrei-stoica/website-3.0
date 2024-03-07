---
title: Rust has a lot to teach other languages
categories:  
        - rust 
        - learning
date: "2023-06-20"
---

Recently, I decided to pick up Rust. While I'm not yet 100% comfortable with the
language, I have had one major takeaway from the experience. The new developer
experience for all other languages is trash!

We all know the saying "Necessity is the mother of invention", but man does it
ever ring true here. It's clear! Rust being as hard as it is to learn
forced that team to create the best possible introduction to it. When you go to
the [Rust-Lang](https://www.rust-lang.org/) website there are three ways to get
started under the [learning](https://www.rust-lang.org/learn) tab.


First, there is ["Read the book"](https://doc.rust-lang.org/book/).
There are plenty of books that serve as introductions to programming languages.
This isn't the interesting part. However, I did find this well written with good
example code and I do recommend people at least skim this and probably use it as
a supplement to the other learning methods I will mention later.

Next is the ["Rustlings"](https://github.com/rust-lang/rustlings/) course.
Here is where it gets interesting. This is an interactive course where you are
given a program that doesn't compile and you need to determine how to fix it.
There are exercises for starting with variables and control flow and going all
the way up to error handling, generics and unique rust features like traits and
lifetimes.

To run through the exercises you can clone the repo and install it with Rust's
package manager. Then running `rustlings watch` will automatically compile the
exercise code and run it for you. Each exercise has a line that you will need to
remove to move on to the next exercise. This can allow you to play around with
different solutions once you have completed an exercise.

I found this sort of compiler-driven teaching style very effective at getting me
familiar with not only the language itself but also the compiler and the
resources to reference when I encounter other problems down the line. When you
are stuck, the course has a help command that you can run. This will point you
to the correct resource for that exercise. Additionally, there is a readme that
links each of the sections of the course to the accompanying section in the book.

The last option they offer for getting started is "Rust by Example". Here there
are listing with example code for many different tasks. Again this could be
anything from a simple hello world to the complicated rust specific features
like traits and lifetimes. But it also contains testing and examples from the
standard library. This will be a more useful resource later when trying to use
the standard library and building some larger projects.

In my opinion, the real star of the show here is **Rustlings**. The fact that it
forces you to install and familiarize yourself with the tool you will be using
from day 0 is beautiful. While there are books that walk you through all of the
same things for other languages and similar courses online are available, this
is the first time I've seen something like this from the developers of the
language itself. Additionally, this is all freely available on GitHub and their
website. 

When you're done with the course and need to dive deeper they also have links on
that same page for:
- standard library
- differences between editions
- package manager
- documenting your code 
- the compiler

as well as application specific books:
- command line application
- webassembly
- embedded programming

Again all of this is **FREE** on the language's website. This is not only a great
beginner introduction but it also gives you great ideas for projects to boost
your proficiency after you get your footing. 

In 2023, it's nice to see a language taking the newcomer experience so seriously
and thinking about the path to proficiency. I think this sort of system for
learning would benefit other languages and would love to see it mirrored. 

I think most people would agree that Clojure is another modern language that can
be difficult to learn. Despite it being similarly difficult, the newcomer
experience is nowhere near as nice. One thing both of these share is the ability
to use the language right in the browser. That's nice but it still doesn't get
you familiar with the rest of the ecosystem and the compiler. If you even want a
tool to help manage the dependencies of your project, you'll have to find your
way to [Leiningen](https://leiningen.org/) on your own somehow. Now let's look
at how the Clojure maintainers expect a new person to learn. Under the
["How do I learn the language"](https://clojure.org/guides/getting_started#_how_do_i_learn_the_language)
section, there is a basic written guide introducing you to the language akin to
the book that Rust provides. Next, there are 4 books that you can pay money for.
A set of problems you can solve interactive in the browser. There is a course
you can sign up for that also has mentors.

I'm not saying these are bad options to start on a new language. For those
who prefer learning from books, I'm sure it works. For those who can afford to
buy the books, I'm sure it works. But for students, for those between jobs, the
fact that Rust offers such a comprehensive view of the ecosystem for free is
fantastic.

I find that following examples from a book doesn't put me in the same
exploratory mind space as the Rustlings course did. With a book in front of you,
the answer is always there as well. Further down the page or on the following
one. All you need to do is keep reading. With the course, you need to explore
to find the solution. When you find it, you're already thinking of other
possible solutions. This encourages you to keep thinking. Running the help
command points you to the right answer but doesn't hand it to you. It still
forces you to process and understand the documentation The fact that you need
to swap your attention from the editor to a browser means that you are less
likely to do it since it requires a context switch. With the book method, you
are already encouraged to switch back and forth so it's no big deal to do it
one more time.

If you haven't done so already, check out the
[Learn](https://www.rust-lang.org/learn) page of the Rust website. It is a
lesson in making that is notoriously difficult accessible. Other languages,
new and old, should take a lesson from their playbook.
