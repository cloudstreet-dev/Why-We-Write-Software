# Chapter 3: Why We Write Games (And Why We Can't Stop)

In 1962, a group of MIT students had access to one of the most expensive machines on the planet: a PDP-1 computer, worth about $120,000 (roughly $1.2 million in today's money). This machine could calculate missile trajectories, model nuclear reactions, or process complex data for scientific research.

They used it to write Spacewar!, a game where two spaceships shoot at each other while trying not to fall into a gravity well.

This tells you everything you need to know about programmers.

## The First Waste of Time

Let's be honest: from a purely utilitarian perspective, games are a waste of computing resources. They don't cure diseases or predict weather or balance budgets. They exist solely to entertain, to amuse, to create experiences that vanish the moment you close the program.

And yet, games were one of the first things we wrote software for. Not business applications. Not productivity tools. Games.

Why?

The official answer is that games are good for testing hardware, for pushing the boundaries of what computers can do, for developing algorithms that later find "serious" applications. This is true. Graphics rendering, physics simulation, artificial intelligence, network optimization—all of these advanced significantly because game developers needed to make things look cool and run fast.

But the real answer is simpler: games are fun to write.

There's a special joy in making something playful, in creating a little universe with its own rules, in crafting experiences that make people laugh or gasp or curse at their screen. It's the same joy that children feel when they make up games on the playground. We're not solving important problems. We're just playing.

And play, it turns out, is deeply important.

## The Taxonomy of Fun

Not all games are created equal, and not all games scratch the same itch. Over the decades, we've written millions of games, and they tell us something about what humans find satisfying.

**Puzzle games** appeal to problem-solvers. Tetris is just fitting shapes together, but it's also one of the most successful games ever made. Why? Because it creates a flow state—that perfect balance between challenge and skill where time disappears and you're fully absorbed. We write puzzle games because we like creating those "aha!" moments, those elegant solutions that feel inevitable in hindsight.

**Action games** appeal to our reflexes and spatial reasoning. Every first-person shooter, every platformer, every bullet-hell game is testing the limits of human reaction time. We write action games because it feels good to master difficult controls, to achieve precision, to pull off the impossible move. Also, explosions.

**Strategy games** appeal to planners and tacticians. Chess is a strategy game. So is Civilization, where you guide a nation from the Stone Age to the Space Age, making thousands of small decisions that compound over hours of play. We write strategy games because we enjoy creating systems complex enough to be interesting but comprehensible enough to master.

**Role-playing games** appeal to storytellers and character-builders. You're not just playing; you're inhabiting a character, making choices, living out a narrative. We write RPGs because we want to create worlds, to tell stories, to give players agency in a narrative. Every RPG is a DM's campaign scaled up, automated, and distributed.

**Simulation games** appeal to tinkerers and managers. SimCity lets you build a city and watch it grow. The Sims lets you control people's lives in disturbing detail. Flight simulators let you crash expensive aircraft without consequence. We write simulation games because reality is constraining, and it's fun to see what happens when you give players god-like powers over a small domain.

**Social games** appeal to our need for connection and competition. MMORPGs, multiplayer shooters, online poker—these games are barely about the mechanics. They're about the people. We write social games because humans are social creatures, and games give us structured ways to interact, compete, cooperate, and form communities.

Each type of game requires different skills to build, but they all share something: they're systems that create experiences. And creating experiences is what makes game development addictive.

## The Game Dev's Curse

Here's something they don't tell you about game development: it ruins games for you.

Once you know how games work—once you've implemented collision detection, written an AI opponent, debugged pathfinding algorithms, balanced stats for hundreds of hours—you can't play games innocently anymore. You notice the seams. You see where the designer made compromises. You spot the tricks they used to save memory or processing power.

You're watching a beautiful cutscene and you're thinking, "I bet that's pre-rendered." You're enjoying a boss fight and you're thinking, "Interesting that they scripted health-based phase transitions instead of time-based." The fourth wall is permanently broken.

And yet, game developers play more games than anyone else. Because we're studying. Because we're looking for ideas to steal. Because even though we see the magician's tricks, we still appreciate the artistry of a well-executed illusion.

There's also a specific type of masochism unique to game developers: we play games to criticize them. "I could do better," we think, even though we probably couldn't. "Why did they make that choice?" we wonder, while making equally questionable choices in our own projects.

Game development is the only form of software development where your users are also critics, where they have strong opinions about frame rates and control responsiveness and whether the ending was satisfying. Game developers get feedback like "this game changed my life" and "this is trash and you should feel bad" about the same product, sometimes on the same day.

## Why Games Are Hard

Writing a game is writing several complex systems and making them all work together in real-time:

You need a **rendering engine** to draw things on screen. This means understanding 3D mathematics, shaders, textures, lighting, camera systems. Or you use someone else's engine and spend weeks learning its quirks.

You need **physics** if anything moves or collides. This means implementing vectors, collision detection, response forces, friction, gravity. Or you use a physics library and spend weeks debugging why objects sometimes fall through the floor.

You need **input handling** that feels responsive. This is harder than it sounds. Players can tell when there's a 50-millisecond delay between pressing a button and seeing a response. They can feel when movement isn't quite right. "Game feel" is notoriously difficult to quantify and even harder to implement.

You need **AI** for enemies, NPCs, or computer opponents. Game AI is its own discipline, distinct from machine learning or "real" AI. It's not about being smart; it's about being fun to play against. Too difficult and players quit. Too easy and they're bored. Too predictable and they exploit patterns. Too random and it feels unfair.

You need **state management** to track everything: player position, inventory, quest progress, enemy status, world changes, save data. Get this wrong and you get bugs like "I fell through the world" or "my save file corrupted" or "the boss became invincible."

You need **audio** that synchronizes with gameplay, creates atmosphere, and doesn't drive players insane. Sound design is an underappreciated art. The right sound effect makes an action feel powerful. The wrong one breaks immersion.

You need **UI/UX** that's intuitive, attractive, and gets out of the way. Every button, every menu, every popup needs to be designed, implemented, and tested. Bad UI kills good games.

And you need to make all of this run at 60 frames per second (or 30, or 120, depending on platform and ambition), on hardware you don't control, for players who will try things you never imagined.

Oh, and it needs to be fun. That's the hard part.

## The Indie Dream

Something magical happened in the 2000s and 2010s: game development became accessible.

You no longer needed a team of 50 people and a million-dollar budget to make a game. Unity, Unreal Engine, GameMaker, Godot—these tools put professional-grade game development within reach of anyone with a computer and determination.

This unleashed an explosion of creativity. One-person studios created breakout hits. Minecraft started as one developer's hobby project. Stardew Valley was made by one person over four years. Undertale, Papers Please, Braid, Limbo—small teams creating innovative, memorable games.

The indie game scene proved that you don't need photorealistic graphics or Hollywood voice acting to make something people love. You need a good idea, solid execution, and usually one unique mechanic or emotional core that AAA studios wouldn't take a risk on.

But here's the dark side: for every successful indie game, there are thousands that nobody plays. The Steam store adds dozens of new games every day. Standing out is nearly impossible. Most indie developers lose money. The ones who succeed are talented, yes, but also lucky.

The indie dream is beautiful and brutal in equal measure. It's beautiful because anyone can try. It's brutal because most will fail. But people keep trying anyway, because the alternative—not making games—is worse.

## Why We Can't Stop

Game development is objectively irrational. The hours are long. The pay is often worse than other software development. The job security is terrible—studios close without warning. The crunch culture is toxic. The players can be ungrateful or hostile.

And yet there's a waiting list of people who want to break in.

Why?

Because games are magic. Because creating joy is addictive. Because seeing someone play your game—really play it, get absorbed in it, care about it—is a feeling that doesn't exist anywhere else in software development.

When you write a database, nobody talks about it at dinner parties. When you optimize a checkout flow, nobody writes fan fiction about it. When you fix a bug in enterprise software, nobody creates fan art.

But games? Games enter culture. People cosplay as your characters. They create mods and maps. They speedrun your levels. They debate your story choices. They remember your game years later and tell other people about it.

This is the real reason we write games: because we want to create experiences that matter to people. We want to build the thing that someone remembers playing when they were twelve, the game that got them through a difficult time, the world they escaped into when reality was too much.

Every game developer has a story about the game that made them want to make games. Mine was—well, that's not important. What's important is that we're all trying to recreate that feeling, to pass it on, to be the reason some kid decides they want to make games too.

## The Eternal Question

"Is it fun yet?"

This is the question that haunts every game developer. You can write perfect code, create beautiful art, design intricate systems, and still end up with something that isn't fun to play.

Fun is emergent. It comes from the interaction of systems, from the balance of difficulty and reward, from the hundred tiny details that create flow. You can't engineer fun directly. You can only create the conditions for it and hope.

This is why game development is so frustrating and so compelling. You're trying to create an emotional state in another person using logic and mathematics. You're trying to make someone laugh by arranging pixels in the right order. You're trying to create tension and release, challenge and triumph, fear and relief, all through the manipulation of bits in memory.

It shouldn't work. But sometimes it does, and when it does, it feels like you've discovered a secret about how human minds work.

## In Defense of Waste

Games are, ultimately, a waste of resources. They consume electricity to create ephemeral entertainment. They occupy developer time that could be spent on "important" software. They distract billions of people from productive activities.

Thank goodness.

Because humans need play. We need stories. We need challenges that don't matter, risks that aren't real, victories that are meaningless but still feel good. We need ways to connect with friends, to test ourselves, to explore impossible worlds.

Games give us a safe space to fail, to learn, to try new identities, to make choices and see consequences. They're practice for life, even when they're completely unrealistic. They're social glue, even when played alone. They're art, even when they're silly.

We write games for the same reason ancient people carved game boards into stone, the same reason medieval people played chess, the same reason children play pretend: because play is how humans make sense of the world.

And we can't stop writing them for the same reason we can't stop playing them: because the next game might be the one that gets it exactly right. The perfect balance, the perfect feel, the perfect experience.

It probably won't be. But we'll keep trying anyway.

Because that's what game developers do.

---

*Next: Chapter 4 - [Software That Pays the Bills](chapter-04-pays-the-bills.md)*
