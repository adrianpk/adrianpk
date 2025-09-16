# What is Going On?

Most of what’s visible here represents spare-time work. I’m a single developer, and public repos capture fragments of ideas that live across different projects. Some of them already exist in repeatable forms, just not as cleanly or ergonomically as I’d like. The goal is to consolidate what feels most solid and reusable, at a pace that makes sense. There are no external demands to meet, only the process of refining what lasts.

Lately I’ve been working around two main threads that explore different approaches to Go code generation.

[HatMax](https://github.com/hatmaxkit/hatmax) and [Pulap](https://github.com/pulap/pulap) move together. HatMax generates microservice monorepos from a declarative spec, focused on plain Go with no hidden dependencies. Pulap is the reference implementation, a real estate management system where those ideas are tested before being folded back into the generator.

[Aquamarine](https://github.com/aquamarinepk/aquamarine) and its companion lib [aqm](https://github.com/aquamarinepk/aqm) follow a similar pattern but from a different philosophy. While HatMax emphasizes total ownership (no imports, every primitive generated into the repo), Aquamarine aims for a more ergonomic approach, centralizing invariants in `aqm`. Code is explicit, wrapping shared components only when needed. In practice, I've been leaning toward Aquamarine for most work. I still prefer the idea of dependency-free code that HatMax embodies, but my development pace is noticeably faster with Aquamarine, and the resulting projects stay lighter since much of the production and test code lives in `aqm` itself. [Appetite](https://github.com/appetiteclub/appetite) acts as its reference implementation, exploring restaurant management use cases while shaping the new iteration of the generator.

I’ve been rotating between these projects at a natural pace. When one takes focus, the others slow down for a while, though none are ever abandoned. Each returns to motion when its time feels right.

Recently, I've also been experimenting with [Aurapack](https://github.com/aurapack/aurapack), a home automation project born from curiosity and frustration in equal measure. It aims to run locally without relying on external servers: speech on a Raspberry Pi, reasoning on a home server, sensors and actuators over MQTT. It mixes Go services with C++ components for voice processing, TTS, STT, and light LLM integration. Don't expect frequent updates here; it's mostly a personal exercise, though I'd love to have more time to shape it into a viable solution. For now, progress will be slow, as it's also a way to reconnect with hardware and bring modern C++ back into my toolset.

[Snapfig](https://github.com/adrianpk/snapfig) is a configuration versioning tool that copies dotfiles and system configs to a git-backed local vault. Unlike symlink-based managers, it keeps actual copies in their original locations, offering real local redundancy. It's feature complete and part of my daily workflow, though I still revisit the implementation from time to time; there's always something that can be refined.

There's also [Tyn](https://github.com/adrianpk/tyn), a minimalist CLI for capturing notes and tasks directly from the terminal. It has been quiet for a while but still forms part of my personal setup, and I plan to fold in some private features once they are ready. Small, fast, and focused, it remains a piece I’d like to refine further.

There are also smaller repositories I revisit from time to time. They serve as refreshers ways to shift focus when there’s a spare moment, always without expectations or deadlines. Like the rest, they move forward when I do.
