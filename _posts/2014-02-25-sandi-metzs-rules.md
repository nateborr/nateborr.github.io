---
title : "Sandi Metz's Rules" 
layout: post
date: 2014-02-25 23:20:00
---

Sandi Metz gave a half-hour talk about rules yesterday at New Relic's Portland office, which I'm happy I could attend. Surely New Relic will publish a video of it shortly, but in the meantime there's a [recording](http://youtu.be/npOGOmkxuio) of an earlier instance of the presentation she gave at Barcelona Ruby Conference 2013.

It's worth any programmer's time. Metz speaks with clarity and incisiveness, sometimes verging on moral gravity, on issues of software quality and maintainability, but without ever losing focus on cost and pragmatism.

The concrete rules she gave are rules for Ruby and Rails apps — "Sandi Metz's Rules", as she ruefully accepts them — are five points that she gave near the end of her epic guest appearance on [Ruby Rogues](http://rubyrogues.com/087-rr-book-clubpractical-object-oriented-design-in-ruby-with-sandi-metz/):

1. No more than 100 lines of code per class.
2. No more than 5 lines per method.
3. No more than 4 parameters per method.
4. No more than 1 instance variable per Rails view.
5. No more than 2 class names per Rails controller.

Metz's stated reason for creating the talk is to reclaim ownership of these rules that are circulating in the world with her name on them, and of the conversation around them. In her telling, the rules have been imperfectly passed on by herself and others, but their precise details are also arbitrary. Teams have had success enforcing both stricter and laxer forms than these. What matters is that the rules will force programmers to create more objects without long stretches of procedural code and, when they inevitably chafe against their boundaries, provoke them to think more carefully about design than they otherwise would have.

More than that, Metz wants to reclaim the level at which this conversation about rules is happening. Bookending her account of what rules to follow was a discussion of what kinds of rules people follow and why they follow them at all. In particular, the third major section of her presentation describes a study that casts rule-following as a way for cooperative individuals to identify and mutually enrich each other, but also as a fragile behavior that's easily disrupted by a single rule breaker. Along those lines, Metz describes declining code quality as a tragedy of the commons. Yesterday she had fewer concrete recommendations, necessarily, for maintaining a healthy software team than for how to structure application code; mainly she impressed on me that we should be careful, somehow, to keep exclusively self-interested programmers from joining our teams in the first place, and try harder to describe what's going wrong when a coworker is sacrificing present and future code quality for the appearance of their own productivity.

Happily, that plays a much smaller part in my day-to-day work life than the need to keep new feature development efficient and sane. My most immediate takeaway from Metz's talk (and from my reading so far of her book [_Practical Object-Oriented Design in Ruby_](http://www.poodr.com/), similarly bracing through its first 100 pages) is to work to keep my code in line with her five rules above, in spirit when not in letter. (In the context of a big legacy app, my early going has involved a fair amount of compromise and a triage mentality.) As a programmer on a small development team, I prefer to use myself as a guinea pig rather than make dramatic proclamations about unfamiliar process changes — but since a couple of the other developers were at the event too, I think we'll find out quickly if the group's collectively interested in a trial run at mass adoption of some new rules.
