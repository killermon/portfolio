# Introduction

I am a senior engineer with 17 years’ experience designing and operating large-scale cloud platforms serving tens of millions of users.

I specialise in system reliability, performance optimisation, and debugging complex issues across the full stack—from Linux kernel and dataplane behaviour through to distributed application design.

Alongside my professional work, I build systems-focused projects in C# and Lua, applying the same principles of performance, scalability, and architectural clarity. These projects serve as a sandbox for exploring low-level design, reinforcing my approach to building resilient, high-performance systems in production environments.

*** This is just a snapshot of the projects I have worked on over the years, to handle all manner of engineering problems. ***

## Tempormental - C# Unity Game.

Tempormental is a systems-driven simulation game built in Unity using C# and the Entity Component System (ECS) framework. The project was designed to consolidate and apply my previous experience into a single, more complex system.

Working with ECS introduced significant challenges due to its evolving API and paradigm shift toward data-oriented design. This required adapting to breaking changes while structuring systems for performance, scalability, and multithreading. I designed systems to remain performant under increasing simulation complexity using Unity’s ECS and Job System.

The project focuses on building interconnected simulation systems, including:

* Atmospheric simulation — models pressure and gas composition (O₂, CO₂, etc.), with dynamic environmental effects
* Structural integrity system — pressure differences can cause hull breaches and cascading failures
* AI behaviour systems — agents react dynamically to environmental changes (e.g. escaping ruptures, interacting with station systems)
* Logistics & pathfinding — AI can transport resources across complex, potentially disconnected station layouts
* Power and gas networks system — distributed systems for resource transport across the station
* Procedural generation — asteroid generation using Voronoi and Perlin noise
* Station construction system — modular building with AI-driven assembly

My main takeaways from this project have been:

* Data-oriented design principles
* Multithreaded system architecture
* Managing complex, interdependent systems
* Designing scalable game logic under performance constraints

👉 Play it [here](
https://play.unity.com/en/games/6a2ce621-87fa-405d-9672-f46760448305/builds)


## Marvin

Marvin has been a key project in my current job role. I was concerned with our current platform deployments, and the consistancy on configuration, and the end result that can have on the customer experience. To this end, Marvin was the solution I engineered to solve this problem.

* Data Moddeling - Creating robust data models to capture the differences between the different versions of our platform, to ensure configuration consistancy.
*  Ease of development - Making development as easy as possible, with a team of engineers who may be unfamiliar with software engineering. Written in Ansible, to make contributing to it as easy as possible.
* Documentation - The goal of this tool was to reduce the dependancie on individuals, myself included. Ensuring the tool was documented at length was an important aspect to achieve this.
* Structure - Aligning with the ease of development goal, ensuring that the structure of the project, including its modules and how it is laid out, to reduce the learning curve for contributing to the project as much as possible.

My main takeaways from this project have been:

* The important of addressing approachability to development.
* Useful abstraction through robust data models, with the appropriate guardrails and validation.
* How to sell a project to the team, ensuring that we collaborate on it, and involve the team within the project. To avoid them feeling like the project is being "forced" on them.

## [BB] Community - Mulitple multiplayer game servers

I've been a developer at this community for 15+ years, with a community that has served over 400,000 players. Made up of various gamemodes, I have written complex systems that underpin the economy of the game, amongst many other facets. The largest challenge with this project has been maintaining the 16.66 Ms tick time, which is the maximum time allowed for code to execute in a single frame - exceeding this would result in the server starting to "Lag", impacting the player experience.

* A cross-server marketplace - players could sell, buy and bid on items in real time. Dealing with ephemeral servers, backed by a common shared database, where players could be logged into multiple servers at once.
* Realtime gameplay feedback systems - Players could see their times in races, in real time, allowing players to know where they are compared to all other players across all our servers.
* Multiplayer cosmetics system - Syncing of equipped cosmetic between players, handling complex data structures to achieve this between the server, and all connected clients. Keeping all clients in sync with one another, as well as optimisations to their rendering pipelines, to handle large amounts of costmetics equipped by players.


My main takeaways from this project have been:

* Players will do things that are undesirable, either maliciously or otherwise.
* Listening to player feedback, and actioning it.
* Player experience, with strict SLA's the amount of time we can spend on the CPU within each frame.
