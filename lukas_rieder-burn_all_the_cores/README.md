# Burn all the cores!

The talk is about a stateful application server built on top of JRuby/JVM.
We at Wooga have built and evaluated such an application server, and now I want to share the learnings and obstacles that came up during development.

**Scaling up:**
We aim to fully utilize our available hardware. One box has 32 Cores and more than 32GB RAM available.
How to saturate such beasts? Well, since JRuby supports real Threads we can share state *(uh oh!)* and saturate cores.

**Scaling out:**
What are the options for scaling a stateful application server?
How to shard state across many servers safely?

I aim for a talk that gives useful tips and shows code. Basically a ratio between 30% background information, 70% showcasing.

**The talk will cover the following topics:**

* Safely sharing state in a concurrent environment using JRuby
* Using Java concurrency utils in JRuby
* Practical tips for tuning JRuby/JVM for maximum throughput
* Practical tips for evaluating performance tunings
* Bonus: Timetraveling

## Lukas Rieder

![Profile picture](http://imgio.heroku.com/fit/150x150/http://profile.ak.fbcdn.net/hprofile-ak-snc6/275767_566192342_1552185551_n.jpg)

I am programming software, and by doing so I want to bring joy and fun to people. That is why I have chosen to work with Wooga. Wooga, is a social gaming company. We <3 the open space and giving learnings back to the community.

Since I started programming, I am curious about concurrency. A couply of years ago, I tried to stay away from shared state the best I could, utilizing databases as centralized data dumps. But now since I have implemented a fully concurrent stateful application server, I am really thrilled by todays possibilities.

I live in Berlin, together with my wife and two children. When I am not just at home being a father, I am programming various stuff. I love to hack on small side projects, especially I love creating small games with paperjs.

## On the web

- [Website](http://lukasrieder.com/)
- [Twitter](https://twitter.com/Overbryd)
- [Github](https://github.com/Overbryd)
