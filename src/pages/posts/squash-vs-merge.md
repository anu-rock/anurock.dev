---
layout: '../../layouts/Post.astro'
title: To merge or to squash on GitHub
description: Using the "squash and merge" option offers some benefits over the "merge commit" option while closing your pull requests.
publishDate: July 30, 2022
featuredImage: '/assets/images/blog/squash-vs-merge/featured.png'
excerpt: 'Using the "squash and merge" option offers some benefits over the "merge commit" option while closing your pull requests.'
tags: ['Dev Productivity']
---

It’s an endless debate.

Like spaces vs. tabs.  
emacs vs. vim.  
Windows vs. Mac.

Before joining Automattic, creating a merge commit was the only way I would close pull requests.
That would get the job done. Perhaps, I thought, the other merge options were for advanced use cases.

Now that I’ve been using the “squash & merge” option extensively for a while, I can better appreciate this option. I think no option is better than the other. Both have their pros and cons.

If you are into carefully crafting all your commit messages — which everybody should be doing anyway — you know the value of a merge commit. It appends all commits of a branch to the target (main) branch. That way, your commit messages are closer to the code they describe. So, each line of code reveals a more precise history with `git blame`.

A squashed commit collates all code changes into a single commit. As a result, commit messages also get consolidated. This can be sometimes annoying as it often results in very large commit messages.

Furthermore, pull requests based on a branch that targets another feature branch will show extra commits from the target feature branch when it’s merged into the main branch. This happens because GitHub automatically adjusts the target branch of the pull request, now pointing it to the main branch. It’s not a blocker, but more than just a minor annoyance especially when there were more than a dozen commits in the target branch.

On the bright side, knowing that all my commit messages would be compacted into one commit allows me to compose shorter, context-free messages.

So, rather than “Add tests for XYZ functionality” I can just write “Add tests” knowing that
the title of my PR would become the first line of the squashed commit that would set the context. So one obvious benefit of using squash & merge is the time you get back from thinking too much about the right commit message.

If you are into the art of creative writing, you’ll find using the merge commit option as a good practice playground.

The rest of us can stick to squashing.

So here it is: squashing deconstructed for you.

Choose wisely!