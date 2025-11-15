# Chapter 1: In the Beginning Was the Bug

The first computer bug was a moth. This is not a metaphor.

On September 9, 1947, engineers working on the Harvard Mark II computer found the machine malfunctioning. They opened the relay panels and discovered an actual moth, wings spread, lodged between relay contacts. Someone on the team—history isn't certain who—taped the moth into the logbook with the annotation "First actual case of bug being found." Grace Hopper was working on the Mark II at the time and later popularized the story, cementing the moth's place in computing folklore.

The joke, of course, is that engineers had been calling problems "bugs" for decades before that moth made its fateful flight. Thomas Edison wrote about bugs in 1878. The term was engineering slang, shorthand for those mysterious gremlins that made things not work. The moth didn't create the metaphor—it just gave us a perfect, literal example of it. Here was a tiny creature that could bring our grand logic to a halt, proof that our machines were vulnerable to the chaos of the physical world.

This is a book about why we write software, but it begins with failure because that's where all software begins. With a problem. With something broken, or something that could be better, or something that doesn't exist yet but should. Every program is born from imperfection—either in the world we're trying to improve, or in our previous attempts to improve it. We write software because the world is full of bugs, metaphorical and otherwise, and fixing problems is what we do.

## The First Programs Were Woven

Before the moth, before the Mark II, before the very concept of a "computer" as we know it, someone had already written the first program. Her name was Ada Lovelace, and in 1843 she wrote an algorithm for Charles Babbage's Analytical Engine—a computer that was never built.

Think about that for a moment. The first program was written for a computer that didn't exist. It was pure thought, pure logic, a solution looking for a machine to run on. Ada understood something profound: the program was separate from the machine. The logic could exist independent of the hardware. She saw that Babbage's engine could manipulate symbols, not just numbers. She imagined it composing music, creating graphics. She saw software before there was software to see.

But even Ada wasn't the first, not really. The first programs were textile patterns on punch cards, fed into Jacquard looms in 1804. The first programmers were weavers. They were writing instructions—if/then logic, loops, conditional branches—into cards that told the loom which threads to lift. They were debugging when patterns came out wrong. They were probably swearing at their machines, too, though the historical record is silent on this point.

The point is: we've been writing instructions for machines since we had machines to write instructions for. And before that, we were writing instructions for each other. Recipes. Musical scores. Architectural plans. Every blueprint, every choreographed dance, every play with its stage directions—these are all programs of a sort. Instructions that, if followed precisely, should produce a specific result.

Should. That's the key word. That's the bug.

## The Electronic Frontier

When the first electronic computers hummed to life in the 1940s, they were programmed by physically rewiring them. The ENIAC, which began operating in 1945, weighed thirty tons and required teams of programmers (mostly women, though history often forgets this) to reconfigure cables and set thousands of switches for each new program. Programming wasn't typing; it was physical labor. A typo wasn't a typo—it was a misconnected wire.

The stored-program computer changed everything. The idea, developed independently by several people (because good ideas are always in the air, waiting to be plucked), was simple but revolutionary: store the program in the same memory as the data. Suddenly, you could change what a computer did without rewiring it. You could write a program to write programs. You could make mistakes faster than ever before.

The 1950s brought us FORTRAN, the first high-level programming language that people actually used. Before FORTRAN, you wrote in assembly language, which meant you were essentially writing directly in the computer's native tongue—moving specific bits to specific registers, one instruction at a time. FORTRAN let you write something almost like English: `IF (X .GT. Y) THEN`. The computer would translate that into the tedious assembly instructions.

Programmers hated it at first. Real programmers didn't need this hand-holding. Real programmers wrote in assembly. They knew their machine. This debate—whether abstraction makes us weak or powerful—would repeat itself at every level, in every generation. Real programmers don't need operating systems. Real programmers don't need high-level languages. Real programmers don't need garbage collection. Real programmers don't need TypeScript.

Spoiler: abstraction won every time, and we still have this argument every time.

## Why Did We Start Writing Software?

The early computers were built for war. The ENIAC calculated artillery firing tables. Colossus broke German codes at Bletchley Park. The first programs were written because people needed to kill each other more efficiently, which is a depressing start to any technology but an honest one.

But almost immediately, we started writing software for other reasons:

We wrote software to **calculate things humans couldn't**. Not just artillery tables, but weather forecasts, nuclear simulations, the trajectories of spacecraft. We wrote software to extend our minds the way telescopes extended our eyes.

We wrote software to **handle tedium**. Payroll. Inventory. Accounting. The business world had rooms full of human "computers"—mostly women, again—doing arithmetic all day. Software could do it faster, more accurately, and without getting bored. It freed humans from drudgery, and also put many of them out of work. This tension has never been resolved.

We wrote software to **play**. The first video game was probably "Tennis for Two," created in 1958 on an oscilloscope by a physicist who was bored. Or maybe it was "Spacewar!" in 1962, written by MIT students who had access to a $120,000 computer and decided the most important thing to do with it was shoot spaceships at each other. We write games for the same reason we've always played games: because reality is hard and we need somewhere else to be for a while.

We wrote software to **prove we could**. Every early programmer has a story about the first program that worked. The first time the computer did exactly what you told it to. There's a specific joy in that, a feeling of power that borders on magic. You typed words, and reality changed. The computer obeyed. This is why children learn to code, and why adults stay up until 3 AM debugging: because making things work feels like casting spells.

## The Cambrian Explosion

By the 1970s, software had escaped the lab. Personal computers arrived—first for hobbyists, then for everyone. The Apple II, the Commodore 64, the IBM PC. Suddenly, millions of people had computers in their homes, and someone needed to write software for them.

This is when everything exploded. People wrote database software, word processors, spreadsheets. VisiCalc, the first spreadsheet program, was called "the software that sold the hardware"—people bought $2,000 Apple IIs just to run this one program. Why? Because it let them ask "what if" questions about their businesses. What if we raised prices 10%? What if we hired three more people? The computer would recalculate instantly. This was new. This was revolutionary.

People wrote games—so many games. Text adventures like Zork, where you typed "go north" and "get lamp" and the computer told you a story. Arcade games. Early RPGs. Flight simulators. Each genre invented new reasons to write software, new problems to solve.

People wrote productivity tools, creativity tools, educational software, utilities, programming languages, operating systems. A thousand flowers bloomed, and most of them died, but the ecosystem grew richer with each extinction.

## And Then the Internet Happened

For most of software's first fifty years, programs were isolated things. They ran on one computer. Maybe they could share data via floppy disk, if you were lucky. The internet—and especially the World Wide Web in the early 1990s—changed the fundamental question from "what can a computer do?" to "what can connected computers do?"

The answer, it turns out, is almost anything.

We started writing software to connect people. Email, chat rooms, forums, social media. We started writing software to share information—websites, search engines, wikis. We started writing software to buy things, sell things, watch things, make things.

The web meant that software could update itself. Could improve continuously. Could scale from one user to a billion users. It also meant that software was never finished, never done, never shipped in the old sense. Your product was your ongoing service. Your code was always running somewhere, and if it broke, everyone knew immediately.

## Where We Are Now

Today, software is everywhere. It's in your pocket, on your wrist, in your car, in your doorbell, in orbit above your head. We write software to predict what you want to buy, who you want to date, what you want to watch. We write software to fly planes, to trade stocks faster than humans can think, to diagnose diseases, to generate text that sounds eerily like a human wrote it.

The scale is staggering. GitHub hosts over 100 million repositories. There are an estimated 27 million professional software developers in the world, and millions more who code as part of their jobs. The Stack Overflow question-and-answer database contains over 20 million questions. More code is written each year than in the entire first half-century of computing combined. We are drowning in code.

And yet, we keep writing more. Why?

That's what the rest of this book is about. But the short answer is: because we have to. Because every problem we solve with software creates three new problems that need software solutions. Because every abstraction layer we build becomes the foundation for the next layer. Because software eats the world, and then needs to eat itself to keep going.

We write software because there's a bug in the world, and we think we can fix it.

Sometimes we're right. Sometimes we just create more bugs.

But we keep trying anyway, because that's what programmers do.

---

*Next: Chapter 2 - [The Cathedral Builders of Silicon](chapter-02-cathedral-builders.md)*
