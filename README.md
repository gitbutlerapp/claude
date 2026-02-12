# GitButler Claude Plugin

> [!NOTE]
> The claude code hooks are no longer the recommended way of integrating with GitHub.
>
> We now recommend using our skill for the `but` CLI. The skill can be installed using `but skill install --global`.

This is a Claude Code plugin that provides a better version control experience than watching your agent struggle with a series of complex Git commands.

## What does it do?

It installs hooks in the Claude lifecycle to automatically stage and commit changes after each Claude Code task is completed.

## Upcoming work : TODO

Soon we will add some cool slash commands that you can use to customize the commit checkpoints that are automatically created:

* `/absorb` - absorbs the last commit into the one before it, if possible
* `/squash` - squashes all commits in the branch into one and rewrites the commit message
* `/commit` - if you've done manual work, creates a commit where you are

Also a number of commands to help open Pull/Merge Requests or update already pushed ones and manage that flow.

Perhaps a subagent that can do more complex branch operations after the fact.

## Installing

To install this plugin for use in Claude Code, add this marketplace and then install the `gitbutler` plugin that it provides.

```
/plugin marketplace add gitbutlerapp/claude
/plugin install gitbutler
```

Once installed, Claude will automatically commit after every completed task.

You will need to have the GitButler CLI installed for this to work:

https://gitbutler.com/downloads

