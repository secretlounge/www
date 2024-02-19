---
title: FAQ
---

# Is this bot really anonymous?

When using the source in [this repository](https://github.com/secretlounge/secretlounge-ng)[^1], unless you reveal yourself,
ordinary users in the bot have zero possibilities of discovering your Telegram user.

Mods and admins in the bot can tell the authors of recent messages
apart (but not the underlying Telegram account) through a
pseudo-random ID returned by the `/info` command. This ID changes
every 24 hours, posts also expire from the cache after 24 hours[^2]
(or if secretlounge-ng is restarted) meaning that they become unable
to be deleted or their authors determined.

People with access to the server the bot runs on have no direct, but a
variety of indirect ways to determine who wrote a particular message.

However, people with access to the bot log file and admin on the bot
can blacklist a user to see the blacklisted user log message[^3]. The
admins of the official secretlounge bots reserve blacklisting for the
most egregious rule violations, almost always for posting illegal
content (a violation of rule 1). A blacklisted user's username is only
disclosed privately to a law enforcement officer presenting a signed
court document. See the [Legal](/meta/legal/) page for more info.

[^1]: It is impossible to ascertain this from afar. You have to trust
    the bot owner either way.

[^2]: Sophisticated attacks are possible to track continously active users over a longer timeframe. It is not expected that a human can perform this.

[^3]: https://github.com/secretlounge/secretlounge-ng/blob/3a668fee5924403af156cc2f155fbda9d1a9bb95/secretlounge_ng/core.py#L470

All of these assessments presume a sufficient user population in the bot so that anyone could blend in.
