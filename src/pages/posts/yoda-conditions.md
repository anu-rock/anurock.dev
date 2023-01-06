---
layout: '../../layouts/Post.astro'
title: Yoda conditions
description: Yoda notation is a style of writing conditions, especially equality checks, in reverse order.
publishDate: January 6, 2023
featuredImage: '/assets/images/blog/yoda-conditions/featured.png'
excerpt: Yoda notation is a style of writing conditions, especially equality checks, in reverse order.
tags: ['Dev Bytes']
---

*Prefer video format? [Watch it on YouTube.](https://youtu.be/9WJgfMaExy0)*

In software development, references to popular culture are not uncommon. Programmers tend to be nerdy fans of superhero and sci-fi genres.

Yoda conditions, aka Yoda notation, is a style of writing conditions, especially equality checks, in reverse order. The name comes from one of the most memorable characters in Star Wars called Yoda.

Yoda is arguably the wisest and most powerful Jedi ever, but he speaks sentences with words in a strange order. Rather than following the standard subject-verb-object sequence, he says the object before the subject and verb.

Consider the English sentence, “The mind of a child is truly wonderful.” This is how Yoda will say it - “Truly wonderful, the mind of a child is.” In fact, he said it in Episode 2 - Attack of the Clones.

To apply Yoda’s style to programming, when comparing the value of a variable, rather than writing “person_age double-equals 29”, you write “29 double-equals person_age”.

If that sounds weird, you are not alone. Programmers usually find it difficult to adjust to this “unnatural” style of writing conditions. You might be thinking, “if it’s so difficult to read why do we write it in the first place?”

To be fair, this style is not simply a cool way of writing conditions. It protects programmers from a common beginner’s mistake of doing a variable assignment when equality was intended. So, in an if-condition, writing “person_age single-equals 29” instead of double-equals may have drastic consequences. By writing the value first, we can easily avoid this trap.

Yoda conditions are popular in PHP and JavaScript communities and less popular or discouraged in other languages. WordPress and Symfony are the two most prominent proponents of this style and have it baked into their coding standards.

Although I am a big fan of the Star Wars franchise, I dislike Yoda conditions. When taken too far, they can make code quite unreadable for me. I know many others who share the same sentiment. Uncle Bob once said, “Code that protects the author at the expense of the reader is flawed code.” I cannot agree more.