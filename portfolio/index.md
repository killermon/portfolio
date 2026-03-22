# Introduction

I am an experience hobbyist game developer with 17 years experience in different conexts. This has involved working within the Unity game engine in C#, within GarrysMod in Lua, as well as a number of other projects not related to gaming I have done through my career at BT. Through my time seveloping software, it has been experienced by over 400,000 people. This has given me a unique view as to how people interact with software, in both expected, and unexpected ways, including dealing with bad actors.

Outside of work, my projects are pricipally written both to learn, but also to turn any ideas I have into reality. This is also then tempered by working in a game community, where any implemented software features, need to be of benefit to the community and help with player retention. I enjoy using projects as a way of pratically extending my skills, and real world problem solving.

## Tempormental - C# Unity Game.

Tempormental is a systems-driven simulation game built in Unity using C# and the Entity Component System (ECS) framework. The project was designed to consolidate and apply my previous experience into a single, more complex system.

Working with ECS introduced significant challenges due to its evolving API and paradigm shift toward data-oriented design. This required adapting to frequent breaking changes while structuring systems for performance, scalability, and multithreading. I designed systems to remain performant under increasing simulation complexity using Unity’s ECS and Job System.

The project focuses on building interconnected simulation systems, including:

* Atmospheric simulation — models pressure and gas composition (O₂, CO₂, etc.), with dynamic environmental effects
* Structural integrity system — pressure differences can cause hull breaches and cascading failures
* AI behaviour systems — agents react dynamically to environmental changes (e.g. escaping ruptures, interacting with station systems)
* Logistics & pathfinding — AI can transport resources across complex, potentially disconnected station layouts
* Power and gas networks — distributed systems for resource transport across the station
* Procedural generation — asteroid generation using Voronoi and Perlin noise
* Station construction system — modular building with AI-driven assembly

This project strengthened my understanding of:

* data-oriented design principles
* multithreaded system architecture
* managing complex, interdependent systems
* designing scalable game logic under performance constraints

👉 Play it [here](
https://play.unity.com/en/games/6a2ce621-87fa-405d-9672-f46760448305/builds)


## [BB] Community

I've been a developer at this community for 15+ years, with a community that has served over 400,000 players. Made up of various gamemodes, I have written complex systems that underpin the economy of the game, amongst many other facets. The largest challenge with this project has been maintaining the 16.66 Ms tick time, which is the maximum time allowed for code to execute in a single frame - exceeding this would result in the server starting to "Lag", impacting the player experience.

* Creating a cross-server marketplace, where players could sell items. Dealing with ephemeral servers, backed by a common shared database, where players could be logged into multiple servers at once.

## Marvin

Marvin has been a key project in my current job role. The engineer goal of this project was to solve the issue of ensuring our Openstacl Cloud was consistantly deployed. Our current automation solution was able to deploy this software, but it often wasn't consistant. This project used custom data modelling to align with our internal platform versioning, and was written in Ansible. Ansible was picked as although it wasn't the most suitable langauge, it allowed other members of my team to pick it up, who didn't have a software engineering background. 