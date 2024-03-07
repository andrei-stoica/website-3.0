---
title: Personal Task Managment  
categories: 
        - todo
        - learning
        - task
date: "2024-03-30"
---

When I was younger and all the things I needed to complete were able to fit in
my head, I was always confused by people who wrote things down, made lists and
crossed them off methodically. I kept hearing about how writing things down
with systems like the [bullet journal](https://bulletjournal.com/) or
[obsidian](https://obsidian.md/) helped people clear their minds. Things didn't
seem that complicated to me. Everything could fit in my head and the few things
that had hard due dates went into my calender. All these systems I heard of
just had too much going on. I had to memorize the system on top of what I
already had going on in my head.

What I didn't realize at the time was that whatever system you use has to be
personal to you. The system you use needs to fill in you're personal week spots.
It needs to be a foundation that you can lean on when your floor starts to
shift. What I was hearing when learning about all of these systems was "what
people are doing" and "how it helped." The important part of learning a new
system is the "why am I doing this." The why is the key piece that informs how
useful it can be for you. As I gain more experience, I learn to focus less on
"whats" and "hows" and more on "whys."

The most important part of personal task management is only the personal part.
Some of you might always want a pen and a list folded in your pocket. Some might
want a fancy to-do app with notifications and reminders. Other's might just use
the notes app that came with your phone. The important part is that you use it
when you need it. No need to have it written down if you just forget the thing
at home or worse you remember the paper but forget the damn pen. Or the other
way around, either way, it somehow feels worse than forgetting both.

For me, most of the things I need to get done happen on the computer. So that's
where I like to keep my list. This has the bonus that when I get up from my
computer I stop thinking about my list of tasks. However, when I am seated at
my desk access I can access them in a few seconds no matter what I am doing.

The system itself is heavily inspired by the bullet journal, which I tried
to do with a physical journal but I found it just sat in my bag untouched after
a while. But, I did start categorizing tasks after that experience.
My 3 categories for tasks are daily, weekly and monthly. These aren't hard
deadlines. They roughly equate to things that need to be done now, things that
are waiting on something else to finish first or are scheduled and things that
I need to start contemplating but not doing. I find that if I don't put any
deadlines on tasks, they don't get done. If everything has a due date they
can overwhelm me. With the combination of these 3 groups, I can focus on the
imminent task, forget about the ones that are blocked and free up time for
those that are around the corner.

Combined with the fact that I can open it without taking my hands off of
the keyboard while working means I am more likely to use the system. Therefore,
the system is more likely to be effective.

I prefer to work in the terminal so I made a system that fits into that
workflow. If I type `todo` in any terminal on my systems, it will open todays
file. If that file doesn't exist, it will take the last file I created, strip
any done tasks and create this new file. The files themselves are markdown. The
editor I configurable, I was using VSCode for a while but I'm currently using
neovim. The tools I use change a lot depending on my day-to-day tasks so I
wanted this to work with whatever editor I choose to use in the future.
For now, I like the speed of neovim. 

The last key to my puzzle is making it available when I am not in a terminal.
That's where a dropdown terminal steps in. Currently, I use
[Guake](https://github.com/Guake/guake) and can open it with `<F12>`. If I don't
already have it open I can type todo to open today's tasks. Usually, I already
have it open as I'm working through tasks on the list and it's only a matter
of opening the dropdown terminal to cross things off and pick the next thing to
do. If I ever start using graphical editors that day-to-day, this could also
work with a key bind that runs `todo` and configuring the utility to open VSCode. 
 

I've written this utility to handle the files and open whatever editor I'm
currently. First in Python then I rewrote it when I started to learn Rust.
The rust version can be found [here](https://github.com/andrei-stoica/rusty-tasks)

Hopefully, there is something you can use here to improve your own system. Mine
is constently evolving. I am currently thinking about adding a new section
to my todo file for notes, and an option in the utility to open the previous day's
files via a flag. That way I can write notes and reference them later. I'm also
trying out Obsidian for something like however I don't think it would be
beneficial to have this split among 2 apps. Another feature I thought could be
useful was to calculate what percentage of tasks get
carried over from day to day. Mapping out my productivity like this could be
insightful but I don't think I doubt it would have the intended effect on me.

The only way I will know how useful any of this can be is to implement it. Then
check back in a month or 2 and the properly useful tools will stay in my
workflow while the rest will be uninstalled from my machine. I look forward to
trying another system in the future and improving my workflow even further.
