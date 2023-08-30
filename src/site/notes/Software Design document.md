---
{"dg-publish":true,"permalink":"/software-design-document/"}
---


# Software Design document

A Software Design Document or Architecture Document is a piece of [[Private/Technical writing\|Technical writing]] that defines a plan for solving a problem with software. It is necessary because software is so complex and requires so many decisions and trade-offs, it cannot be inferred from reading source code.

Should be written by project lead, for projects that take 1 engineer month or more.[^1]

Note that designing a very complex system entirely upfront and expecting it to work generally guarantees failure. Instead, very complex systems that work will emerge over time from simpler systems that work.

## Examples of great documents

Beware, all these examples were written *after* the software was made, and architecture documents are generally written before a project starts. Real architecture documents made for planning are generally kept secret.

- [Audacity](http://aosabook.org/en/audacity.html)
- AWS [This is my Architecture](https://aws.amazon.com/architecture/this-is-my-architecture/?tma.sort-by=item.additionalFields.airDate&tma.sort-order=desc&awsf.category=*all&awsf.industry=*all&awsf.language=*all&awsf.show=*all&awsf.format=*all)
- [[Private/Bash shell\|Bash shell]]'s [Architecture by Chet Ramey](http://aosabook.org/en/bash.html)
- [Git](http://aosabook.org/en/git.html)
- GitLab's [Architecture Overview](https://docs.gitlab.com/ee/development/architecture.html)
- [Rust-analyser](https://github.com/rust-lang/rust-analyzer/blob/d7c99931d05e3723d878bea5dc26766791fa4e69/docs/dev/architecture.md)
- [Selenium](http://aosabook.org/en/selenium.html)
- Stack Overflow, on [Nick Craver's blog](https://nickcraver.com/blog/2016/02/17/stack-overflow-the-architecture-2016-edition/). 

More at [The Architecture of Open Source Applications](http://aosabook.org/en/index.html).

## Components of a design document

### A convenient location and format

Future maintainers will want to read it. Thus it's worth placing it somewhere they can easily read it. One recommendation is to make a file called `ARCHITECTURE.md` in the software repository, adjacent to its `README.md`. [^2]

### Dependencies

Significant files and modules should be mentioned by name, but not linked directly as such links can expire. Searching for the name encourages future maintainers to explore.

### Invariants or exclusions

If you have intentionally excluded something from the design, that thing should be defined along with the reason why. Future maintainers cannot know why something doesn't exist.[^3]

### Diagrams

![C4 diagram for internet banking system](/img/user/Vaults/quartz/content/notes/images/c4_diagram.jpg)

These might be based on the C4 model: context, containers, components, code. Personally I prefer to rename context to *customers*. InfoQ has a [guide to the C4 model](https://www.infoq.com/articles/C4-architecture-model/).

<!-- Eventually the section below should be removed -->

## Guides to writing architecture documents

The open source [arc42 document framework](https://docs.arc42.org/home/) is considered by many to be the best. Features many examples and is entirely free to use. InnoQ has a [guide to using the framework](https://www.innoq.com/en/blog/brief-introduction-to-arc42/).

Free Code Camp has a guide: [How to write a good software design doc](https://www.freecodecamp.org/news/how-to-write-a-good-software-design-document-66fcf019569c/)

https://www.workingsoftware.dev/software-architecture-documentation-the-ultimate-guide/
https://news.ycombinator.com/item?id=34482836

## More reading
https://martinfowler.com/architecture/

[This](https://matklad.github.io/2023/08/06/fantastic-learning-resources.html) says that [this](https://www.tedinski.com/archive/) is good

https://www.workingsoftware.dev/architecture-principles/?ref=refind

https://blog.pragmaticengineer.com/software-architecture-is-overrated/
https://news.ycombinator.com/item?id=21001676

[^1]: "As a general rule of thumb, if you are working on a project that might take 1 engineer-month or more, you should write a design doc. But don’t stop there — a lot of smaller projects could benefit from a mini design doc too." [How to write a good software design doc](https://www.freecodecamp.org/news/how-to-write-a-good-software-design-document-66fcf019569c/)
[^2]: "If you maintain an open-source project in the range of 10k-200k lines of code, I strongly encourage you to add an `ARCHITECTURE` document next to `README` and `CONTRIBUTING`." [ARCHITECTURE.md](https://matklad.github.io//2021/02/06/ARCHITECTURE.md.html)
[^3]: "Explicitly call-out architectural invariants. Often, important invariants are expressed as an _absence_ of something, and it’s pretty hard to divine that from reading the code. Think about a common example from web development: nothing in the model layer specifically doesn’t depend on the views." [ARCHITECTURE.md](https://matklad.github.io//2021/02/06/ARCHITECTURE.md.html)

