Title: This Week in Rust 468
Number: 468
Date: 2022-11-09
Category: This Week in Rust

Hello and welcome to another issue of *This Week in Rust*!
[Rust](https://www.rust-lang.org/) is a programming language empowering everyone to build reliable and efficient software.
This is a weekly summary of its progress and community.
Want something mentioned? Tweet us at [@ThisWeekInRust](https://twitter.com/ThisWeekInRust) or [send us a pull request](https://github.com/rust-lang/this-week-in-rust).
Want to get involved? [We love contributions](https://github.com/rust-lang/rust/blob/master/CONTRIBUTING.md).

*This Week in Rust* is openly developed [on GitHub](https://github.com/rust-lang/this-week-in-rust).
If you find any errors in this week's issue, [please submit a PR](https://github.com/rust-lang/this-week-in-rust/pulls).

## Updates from Rust Community

<!--

Dear community contributors:
Please read README.md for guidance on submissions.
Each submitted link should be of the form:

* [Title of the Linked Page](https://example.com/my_article)

If you don't know which category to use, feel free to submit a PR anyway
and just ask the editors to select the category.

-->

### Official
* [Announcing Rust 1.65.0](https://blog.rust-lang.org/2022/11/03/Rust-1.65.0.html)

### Foundation

### Newsletters

### Project/Tooling Updates
* [rust-analyzer changelog #154](https://rust-analyzer.github.io/thisweek/2022/11/07/changelog-154.html)
* [IntelliJ Rust Changelog #182](https://intellij-rust.github.io/2022/11/07/changelog-182.html)
* [This Month in Rust OSDev: October 2022 | Rust OSDev](https://rust-osdev.com/this-month/2022-10/)
* [This Week in Fyrox](https://fyrox.rs/blog/post/twif/)
* [Cap'n Proto - Generic Associated Types](https://dwrensha.github.io/capnproto-rust/2022/11/03/0.15-release.html)
* [Gitoxide - Cloning the Linux kernel in under a minute](https://github.com/Byron/gitoxide/discussions/579)

### Observations/Thoughts
* [Scoped threads in Rust, and why its async counterpart would be unsound](https://wishawa.github.io/posts/thread-scoped-async/)
* [34 Must Know Terms for Embedded Rust Newbies](https://apollolabsblog.hashnode.dev/34-must-know-terms-for-embedded-rust-newbies)
* [what if pointer properties were in the rust type system](https://cohost.org/myrrlyn/post/197200-what-if-pointer-prop)
* [mmap(1Tb): A Rust arena allocator (ab)using Linux overcommit](https://vgel.me/posts/mmap-arena-alloc/)
* [Contributing to Rust: Bootstrapping the Rust Compiler (rustc)](https://www.youtube.com/watch?v=oG-JshUmkuA)
* [The ‘Viral’ Secure Programming Language That’s Taking Over Tech](https://www.wired.com/story/rust-secure-programming-language-memory-safe/)
* [FR] [series] [Rust par le Métal : move, clone, copy](https://lafor.ge/rust/move/)
* [FR] [series] [Rust par le Métal (Annexe) : Les bases de nombres](https://lafor.ge/rust/annex_bases/)

### Rust Walkthroughs
* [Tauri vs. Electron for Tray Apps](https://betterprogramming.pub/tauri-vs-electron-for-tray-apps-ed15974f35ce)
* [Running Rust in AWS Lambda with SAM — Part 1](https://medium.com/@shyamsundarb/running-rust-in-aws-lambda-with-sam-part-1-2b7a6963a2ef)
* [Tower, Episode 2: calling a Tower Service ](https://heikoseeberger.de/2022/10/23/2022-10-23-tower-2/)
* [Writing an eBPF/XDP Load-Balancer in Rust](https://konghq.com/blog/writing-an-ebpf-xdp-load-balancer-in-rust)

### Research

### Miscellaneous
* [Lynx Joins AdaCore and Ferrous Systems to Bring Rust to Embedded Developers](https://www.lynx.com/press-releases/rust-compiler-support)
* [video] [RUST 1.65 - let-else statements - new language feature!!!](https://www.youtube.com/watch?v=U-5_bumwH9w)
* [video] [The Rust Programming Language for Game Tooling](https://www.youtube.com/watch?v=GtRo-eF8-TE)
* [video] [Bencher—Catch Performance Regressions in CI @ Rust DC, September 20, 2022 w/ Everett Pompeii](https://www.youtube.com/watch?v=Xw9loUatF7k)
* [video] [Impractical Rust: The HATETRIS World Record @ Rust DC, October 18, 2022 w/Dave Freiberg+Felipe Suero](https://www.youtube.com/watch?v=UgQUvD9gyMk)
* [DE] [Programmiersprache Rust 1.65 führt Generic Associated Types ein](https://www.heise.de/news/Programmiersprache-Rust-1-65-fuehrt-Generic-Associated-Types-ein-7329903.html)
* [DE] [Ferris Talk #12: Web-APIs mit Rust erstellen](https://www.heise.de/hintergrund/Ferris-Talk-12-Web-APIs-mit-Rust-erstellen-7321340.html)

## Crate of the Week

<!-- COTW goes here -->

[Please submit your suggestions and votes for next week][submit_crate]!

[submit_crate]: https://users.rust-lang.org/t/crate-of-the-week/2704

## Call for Participation

Always wanted to contribute to open-source projects but didn't know where to start?
Every week we highlight some tasks from the Rust community for you to pick and get started!

Some of these tasks may also have mentors available, visit the task page for more information.

<!-- CFPs go here, use this format: * [project name - title of issue](link to issue) -->
[FOSDEM 2023 Rust devroom CFP](https://rust-fosdem.github.io)
<!-- * [ - ]() -->

If you are a Rust project owner and are looking for contributors, please submit tasks [here][guidelines].

[guidelines]: https://users.rust-lang.org/t/twir-call-for-participation/4821

## Updates from the Rust Project

<!-- Rust updates go here -->

### Rust Compiler Performance Triage

A relatively noisy week (most of those have been dropped below, and comments
left on GitHub), but otherwise a quiet one in terms of performance changes,
with essentially no significant changes occuring.

Triage done by **@simulacrum**.
Revision range: [822f8c2..57d3c58](https://perf.rust-lang.org/?start=822f8c22f540b12f296d844ad5bf39aaa47bfeb4&end=57d3c58ed6e0faf89a62411f96c000ffc9fd3937&absolute=false&stat=instructions%3Au)

2 Regressions, 2 Improvements, 3 Mixed; 3 of them in rollups
39 artifact comparisons made in total

See the [full report](https://github.com/rust-lang/rustc-perf/blob/master/triage/2022-11-08.md) for more details.

### Call for Testing

An important step for RFC implementation is for people to experiment with the
implementation and give feedback, especially before stabilization.  The following
RFCs would benefit from user testing before moving forward:

<!-- Pre-Stabilization RFCs go here -->

<!-- RFC and FCP sections go here -->

## Upcoming Events

Rusty Events between 2022-11-09 - 2022-12-07 🦀

### Virtual

* 2022-11-09 | Virtual (Cardiff, UK) | [Rust and C++ Cardiff](https://www.meetup.com/rust-and-c-plus-plus-in-cardiff/)
    * [**Introduction to Rust Atomics**](https://www.meetup.com/rust-and-c-plus-plus-in-cardiff/events/289052285/)
* 2022-11-09 | Virtual (Darmstadt, DE) | [betterCode](https://www.bettercode.eu/)
    * [**betterCode Rust**](https://rust.bettercode.eu/)
* 2022-11-09 | Virtual (Malaysia, MY) | [Rust Malaysia](https://forms.gle/zWXcMDAnnibiL4ni9)
    * [**Rust Meetup November 2022 - a couple of lightning talks**](https://discord.gg/9Xj8H2EXTD)
* 2022-11-10 | Virtual (Budapest, HU) | [HWSW free!](https://www.meetup.com/hwswfree/)
    * [**RUST! RUST! RUST! meetup (online formában!)**](https://www.meetup.com/hwswfree/events/289044458/)
* 2022-11-10 | Virtual (Nürnberg, DE) | [Rust Nuremberg](https://www.meetup.com/rust-noris/)
    * [**Rust Nürnberg online #19**](https://www.meetup.com/rust-noris/events/hlvbvsydcpbnb/)
* 2022-11-12 | Virtual | [Rust GameDev](https://gamedev.rs/)
    * [**Rust GameDev Monthly Meetup**](https://www.google.com/url?q=https%3A%2F%2Fdiscord.gg%2FyNtPTb2&sa=D&ust=1666661760000000&usg=AOvVaw13uHY9m-8bJJwgeP58VS8l)
* 2022-11-15 | Virtual (Nairobi, KE / New York, NY, US)| [Data Umbrella Africa](https://www.meetup.com/data-umbrella-africa2/)
    * [**Online: Introduction to Rust Programming**](https://www.meetup.com/data-umbrella-africa2/events/289308825/) | [**New York Mirror**](https://www.meetup.com/data-umbrella/events/289308172/)
* 2022-11-15 | Virtual (Washington, DC, US) | [Rust DC](https://www.meetup.com/rustdc//)
    * [**Mid-month Rustful**](https://www.meetup.com/rustdc/events/289015883/)
* 2022-11-16 | Virtual (Vancouver, BC, CA) | [Vancouver Rust](https://www.meetup.com/vancouver-rust)
    * [**Rust Study/Hack/Hang-out**](https://www.meetup.com/vancouver-rust/events/tqvhxsydcpbvb/)
* 2022-11-17 | Virtual (Amsterdam, NL) | [ITGilde Tech-Talks](https://www.meetup.com/itgilde-cooperatie-amsterdam-unix-linux-meetups)
    * [**Introduction “Rust” an ITGilde Tech Talk delivered by Pascal van Dam**](https://www.meetup.com/itgilde-cooperatie-amsterdam-unix-linux-meetups/events/289167373/)
* 2022-11-17 | Virtual (Stuttgart, DE) | [Rust Community Stuttgart](https://www.meetup.com/Rust-Community-Stuttgart/)
    * [**Rust-Meetup**](https://www.meetup.com/rust-community-stuttgart/events/qtvtvsydcpbwb/)
* 2022-11-21 | Virtual (Paris, FR) | [Meetup Paris - École Supérieure de Génie Informatique (ESGI)](https://www.meetup.com/meetup-paris-ecole-superieur-du-genie-informatique)
    * [**Découverte de WebAssembly**](https://www.meetup.com/meetup-paris-ecole-superieur-du-genie-informatique/events/289112753/)
* 2022-11-22 | Virtual (Berlin, DE) | [Berlin.rs](https://berline.rs/)
    * [**Rust Hack and Learn**](https://berline.rs/2022/11/22/rust-hack-and-learn.html)
* 2022-11-24 | Virtual (Linz, AT) | [Rust Linz](https://www.meetup.com/rust-linz/)
    * [**Rust Meetup Linz - 27th Edition**](https://www.meetup.com/rust-linz/events/289251460/)
* 2022-11-29 | Virtual (Dallas, TX, US) | [Dallas Rust](https://www.meetup.com/Dallas-Rust/)
    * [**Last Tuesday**](https://www.meetup.com/dallas-rust/events/qndgwsydcpbmc/)
* 2022-11-30 | Virtual (Munich, DE) | [Rust Munich](https://www.meetup.com/rust-munich/)
    * [**Rust Munich 2022 / 3 - hybrid**](https://www.meetup.com/rust-munich/events/289065390/)
* 2022-12-01 | Virtual (Charlottesville, VA, US) | [Charlottesville Rust Meetup](https://www.meetup.com/charlottesville-rust-meetup/)
    * [**Exploring USB with Rust**](https://www.meetup.com/charlottesville-rust-meetup/events/289563986/)
* 2022-12-06 | Virtual (Buffalo, NY, US) | [Buffalo Rust Meetup](https://www.meetup.com/buffalo-rust-meetup/)
    * [**Buffalo Rust User Group, First Tuesdays**](https://www.meetup.com/buffalo-rust-meetup/events/hlgvxsydcqbjb/)
* 2022-12-07 | Virtual (Indianapolis, IN, US) | [Indy Rust](https://www.meetup.com/indyrs/)
    * [**Indy.rs - with Social Distancing**](https://www.meetup.com/indyrs/events/287027660/)

### Europe

* 2022-11-15 | Tampere, FI | [Rust Finland](https://www.rust-finland.org/)
    * [**Rust Meetup in Tampere**](https://www.lyyti.fi/reg/Finland_Rustlang_Group_meetup_2564)
* 2022-11-16 | Paris, FR | [Stockly](https://www.eventbrite.fr/o/stockly-42274765293)
    * [**Rust Meetup in Paris - hosted by Stockly**](https://www.eventbrite.fr/e/rust-meetup-in-paris-hosted-by-stockly-tickets-444152621447?aff=ebdssbdestsearch)
* 2022-11-23 | Bratislava, SK | [Bratislava Rust Meetup Group](https://www.meetup.com/bratislava-rust-meetup-group/)
    * [**Initial Meet and Greet Rust meetup**](https://www.meetup.com/bratislava-rust-meetup-group/events/289028178/)
* 2022-11-24 | København, DK | [Copenhagen Rust Group](https://cph.rs/)
    * [**Hack Night #31**](https://www.meetup.com/copenhagen-rust-meetup-group/events/288179132/)
* 2022-11-30 | Amsterdam, NL | [Rust Nederland](https://www.meetup.com/rust-nederland/)
    * [**Rust in Critical Infrastructure**](https://www.meetup.com/rust-nederland/events/289204146/)
* 2022-11-30 | Lille, FR | [Rust Lille](https://www.meetup.com/meetup-group-zgphbyet)
    * [**Rust Lille #1**](https://www.meetup.com/meetup-group-zgphbyet/events/289620614/)
* 2022-11-30 | Munich, DE + Virtual | [Rust Munich](https://www.meetup.com/rust-munich/)
    * [**Rust Munich 2022 / 3 - hybrid**](https://www.meetup.com/rust-munich/events/289065390/)

### North America

* 2022-11-10 | Columbus, OH, US | [Columbus Rust Society](https://www.meetup.com/columbus-rs/events/)
    * [**Monthly Meeting**](https://www.meetup.com/columbus-rs/events/dpkhgrydcpbnb/)
* 2022-11-15 | San Francisco, CA, US | [San Francisco Rust Study Group](https://www.meetup.com/san-francisco-rust-study-group/)
    * [**Rust Hacking in Person**](https://www.meetup.com/san-francisco-rust-study-group/events/wjkjssydcpbtb/)
* 2022-11-29 | Austin, TX, US | [ATX Rustaceans](https://www.meetup.com/atx-rustaceans/)
    * [**Atx Rustaceans Meetup**](https://www.meetup.com/atx-rustaceans/events/289594614/)
* 2022-12-01 | Lehi, UT, US | [Utah Rust](https://www.meetup.com/utah-rust/)
    * [**Utah Rust meetup**](https://www.meetup.com/utah-rust/events/dsbpxsydcpbgc/)

### Oceania

* 2022-11-09 | Sydney, NSW, AU | [Rust Sydney](https://www.meetup.com/rust-sydney/)
    * [**RustAU Sydney - Last physical for 2022 !**](https://www.meetup.com/rust-sydney/events/289061840/)
* 2022-11-22 | Canberra, ACT, AU | [Canberra Rust User Group](https://www.meetup.com/rust-canberra/)
    * [**November Meetup**](https://www.meetup.com/rust-canberra/events/288615873/)

If you are running a Rust event please add it to the [calendar] to get
it mentioned here. Please remember to add a link to the event too.
Email the [Rust Community Team][community] for access.

[calendar]: https://www.google.com/calendar/embed?src=apd9vmbc22egenmtu5l6c5jbfc%40group.calendar.google.com
[community]: mailto:community-team@rust-lang.org


<!--

Rust Jobs:

TWiR has stopped featuring individual job postings. You can read more about this change here:

https://github.com/rust-lang/this-week-in-rust/issues/3412

-->

## Jobs

Please see the latest [Who's Hiring thread on r/rust](INSERT_LINK_HERE)

# Quote of the Week

<!-- QOTW goes here -->

[Please submit quotes and vote for next week!](https://users.rust-lang.org/t/twir-quote-of-the-week/328)

*This Week in Rust is edited by: [nellshamrell](https://github.com/nellshamrell), [llogiq](https://github.com/llogiq), [cdmistman](https://github.com/cdmistman), [ericseppanen](https://github.com/ericseppanen), [extrawurst](https://github.com/extrawurst), [andrewpollack](https://github.com/andrewpollack), [U007D](https://github.com/U007D), [kolharsam](https://github.com/kolharsam), [joelmarcey](https://github.com/joelmarcey), [mariannegoldin](https://github.com/mariannegoldin), [bennyvasquez](https://github.com/bennyvasquez).*

*Email list hosting is sponsored by [The Rust Foundation](https://foundation.rust-lang.org/)*

<small>[Discuss on r/rust](REDDIT_LINK_HERE)</small>