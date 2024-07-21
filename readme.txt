download manager with fuse virtual filesystem

file-centric download manager

because download managers should be file-centric

files first

manage downloads like files

organize files in directories

written in elixir for live coding (hot reloading)

https://github.com/mwri/elixir-userfs - fuse in elixir

https://github.com/elixir-crawly/crawly - webscraper in elixir

https://github.com/fredwu/crawler - webscraper in elixir

https://github.com/ryotsu/torrex - bittorrent client in elixir



elixir alternative with static types

https://old.reddit.com/r/elixir/comments/15eld0b/how_to_cope_without_static_types/

  As Joe Armstrong said, a type system wouldn't save your system if it were to get hit by lightning, but fault tolerance would. Let it crash, embrace redundancy and fault tolerance.

  As someone who likes a great type system too, I think pattern matching, guards and typespecs as they currently are already provide a decent experience to reason about input and outputs. Also, new type system is being developed, stay tuned.

  https://github.com/jeremyjh/dialyxir

https://old.reddit.com/r/elixir/comments/9vgjse/elixir_but_with_static_types/

  If you feel like venturing further afield, Rust has a steep learning curve but is very rewarding and has a wonderful community, and there's a very active project called actix that provides an actor system similar to the concurrency model of Erlang/Elixir:

  https://actix.rs

  https://doc.rust-lang.org/book/2018-edition/index.html

    rust live coding?

    https://robert.kra.hn/posts/hot-reloading-rust/

      https://crates.io/crates/hot-lib-reloader

        https://github.com/rksm/hot-lib-reloader-rs

    https://blog.logrocket.com/comparing-elixir-rust-go/

      rust for low memory usage

    https://old.reddit.com/r/rust/comments/2jwgqh/hot_code_reload/

    https://duckduckgo.com/?q=emulating+erlang+in+rust

      # https://github.com/archseer/enigma

      https://github.com/constellation-rs/constellation

      https://github.com/johamb/rust-distributed-programming

      https://github.com/surrealdb/surrealdb

        simplify your database and API infrastructure, reduce development time, and build secure, performant apps quickly and cost-effectively.

        SurrealDB supports SQL querying from client devices, GraphQL, ACID transactions, WebSocket connections, structured and unstructured data, graph querying, full-text indexing, and geospatial querying.

      https://blog.logrocket.com/concurrent-programming-rust-crossbeam/

        concurrent programming in Rust

        it’s possible to build efficient lock-free data structures with Rust,
        but you actually need to build a memory-reclamation mechanism — much like a garbage collector.

          https://github.com/crossbeam-rs/crossbeam

      https://users.rust-lang.org/t/most-complete-and-or-erlang-like-actor-model/93560

        https://github.com/LeonHartley/Coerce-rs

          Actor runtime and distributed systems framework for Rust

        https://github.com/lunatic-solutions/lunatic

          Lunatic is an Erlang-inspired runtime for WebAssembly

        https://github.com/slawlor/ractor

          Rust actor framework

        https://github.com/kvakvs/ErlangRT

          Erlang Replacement Therapy. Another attempt to make Erlang runtime (BEAM emulator) in Rust. Good news: I know what to do. Bad news: I have no clue how to Rust

        https://github.com/rusterlium/rustler

          Safe Rust bridge for creating Erlang NIF functions

        https://old.reddit.com/r/rust/comments/9qe90b/how_to_emulate_the_erlang_process_model/

          Actix might be what you're looking for. It's a library implementing the actor model.

            https://github.com/actix/actix/issues/82

          Tokio, which is an event loop (closer to what you're after) but designed for tasks mostly blocked on IO, and can be rather hard to wrap your head around.

            https://github.com/tokio-rs/tokio

            rust download manager based on tokio

              https://old.reddit.com/r/rust/comments/qn89ad/announcing_dlm_a_minimal_http_download_manager/

                https://github.com/rgreinho/trauma

                https://github.com/agourlay/dlm

                # https://github.com/svmk/rust-network-communicator

            https://duckduckgo.com/?q=rewrite+aria+in+rust

              https://github.com/icanwalkonwater/libaria2-rs

                Rust bindings to libaria2

    rust bittorrent client

      https://github.com/ikatson/rqbit

        https://github.com/NixOS/nixpkgs/pull/306411

    rust webscraper

      https://github.com/spider-rs/spider

        https://github.com/spider-rs/spider-py

    rust fuse filesystem



data pipeline webscraping

  https://www.google.com/search?q=live+coding+web+scraping+hot+reload+data+pipeline

  https://old.reddit.com/r/dataengineering/comments/14hdpg4/how_to_scale_and_automate_webscraping/

    Use python selenium with multi threading and headless browsing to efficiently scrape the websites.
    You’ll also need to incorporate a rotating proxy mechanism to avoid ip blocking and request throttling.
    The reason I say running scraping jobs on multiple threads is that it is far more efficient
    because each thread has an assigned scraping task utilizing all cores of your computer.



language-agnostic data processing pipelines

  https://turbolent.com/data-processing-pipeline

    closed source

    golang

    Instead of reinventing the wheel and building these systems from scratch, we use established off the shelf software:

      Kubernetes: a platform for automatic deployment, scaling, scheduling, and management of containerized applications

      RabbitMQ: a message broker implementing the AMQP 0-9-1 protocol, with support for message queueing, reliable delivery, and flexible routing. It also includes many useful extensions, such as delayed message delivery

    The worker process only communicates with the supervisor via named pipes (FIFO), an extension of pipes which can be used for IPC, through a simple line-based protocol.

  https://github.com/EqualExperts/language-agnostic-data-pipelines

    clojure

  https://github.com/kestra-io/kestra
  https://github.com/SteveAnik/Kestra

    java

    Event-Driven Declarative Orchestrator

    Infinitely scalable, event-driven, language-agnostic orchestration and scheduling platform to manage millions of workflows declaratively in code.

  https://github.com/pditommaso/awesome-pipeline

  https://github.com/topics/workflow-engine

    https://github.com/argoproj/argo-workflows

      Workflow Engine for Kubernetes

      golang

    https://github.com/temporalio/temporal

      golang

  https://github.com/topics/orchestration

    https://github.com/statelyai/xstate

      Actor-based state management & orchestration for complex app logic.

  https://github.com/mattsse/voyager

    crawl and scrape web pages in rust

    state machine

  https://github.com/superstreamlabs/memphis

    data streaming platform

    

webscraping daemon pipeline state machine

  https://medium.com/@lminhkhoa/how-to-build-a-fully-automated-web-scraping-pipeline-for-dashboard-742b6dce9f0f

  https://webscrapingsite.com/resources/building-scraping-pipeline-apache-airflow/

    fav?

    no live coding? no hot reload?

    According to a recent survey by Astronomer, 78% of data teams rely on Airflow for ETL and data integration.

    Visually constructing pipelines makes the logic easy to comprehend.

    https://github.com/kulkarninidhii/webscraping-airflow-pipeline



data processing pipeline "hot reload" error handling interactive

  https://stackoverflow.com/questions/31862167/what-is-a-good-practice-or-design-to-swap-algorithms-at-runtime

    https://en.wikipedia.org/wiki/Strategy_pattern

      In computer programming, the strategy pattern (also known as the policy pattern) is a behavioral software design pattern that enables selecting an algorithm at runtime. Instead of implementing a single algorithm directly, code receives runtime instructions as to which in a family of algorithms to use.[1]

  https://lists.apache.org/thread/yj8ndv97o0ldv10nbn890z7fszt0h5h9

    apache beam

    hot update or hot swap

    I am losing the messages that were being processed in the old
    one and they are not taken by the new one, which imply we are incurring in
    losing data .



data processing pipeline "hot reload" error handling "semi-automatic" "interactive"



arr: automatic download managers

  sources: torrent, usenet. no debrid?

  https://github.com/Ravencentric/awesome-arr

  https://wiki.servarr.com/

   automatically grab, sort, organize, and monitor your Music, Movie, E-Book, or TV Show collections

  https://old.reddit.com/r/selfhosted/comments/1bqwyvk/automated_arr_suite_vs_self_managing/

   prowlarr: Simple search over multiple indexes and I can freely select what to download

   Fileflows (automated transcoding) 



what is the source of truth?

  vbulletin board?

    https://github.com/JeffreyCastellano/forum-scraper

    https://github.com/buengese/scrapy-vbulletin

    https://github.com/vizzerdrix55/web-scraping-vBulletin-forum

  warez blogs?

    https://filmfans.org/

    https://serienfans.org/

  imdb movie lists?


real debrid automation arr

  is usenet better than one click hosters?



semi-automatic web scraping

  meh ...

  https://github.com/AlexMathew/scrapple

    A framework for creating semi-automatic web content extractors

  https://github.com/Yash-Gawai/Semi-auto-web-scraper



https://github.com/topics/scheduler

  https://github.com/apache/airflow

  https://github.com/dagster-io/dagster



high latency everything

  multitasking, parallel processing, many tasks, short attention per task

  start search

  wait for search results

  select downloads from search results

  wait for downloads

  start postprocessing of downloads: unpack, demux, align, compress, remux

  wait for postprocessing, preview results



https://old.reddit.com/r/dataengineering/comments/11nqc61/tencent_data_engineer_why_we_went_from_clickhouse/

  Apache Doris, a real-time analytical database, boasts a few features that are exactly what we needed in solving our problems

  https://github.com/apache/doris


scrapy

  https://dev.to/iankerins/the-5-best-scrapyd-dashboards-admin-tools-42eb

    spider management tools

    ScrapydWeb

      The most popular open source Scrapyd dashboard,
      ScrapydWeb is a great solution for anyone looking for a robust spider management tool
      that can be integrated with their Scrapyd servers.

    Gerapy

      Unlike ScrapydWeb, Gerapy also has a visual code editor built-in.
      So you can edit your projects code right from the Gerapy dashboard
      if you would like to make a quick change.

      https://github.com/my8100/scrapydweb

    Crawlab

      Crawlab is a Golang-based distributed web crawler admin platform for spiders management
      regardless of languages and frameworks.
      Meaning that you can use it with any type of spider
      be it Python Requests, NodeJS, Golang, etc. based spiders.

      https://github.com/crawlab-team/crawlab

rust scripting

  https://github.com/PyO3/pyo3

    Rust bindings for the Python interpreter

    embed python into rust
    call rust from python

  https://github.com/rhaiscript/rhai

    Rhai - An embedded scripting language for Rust.

https://github.com/Gerapy/Gerapy



virtual filesystem

  https://github.com/StrumentiResistenti/Tagsistant

    tags, queries



download manager

  https://github.com/rgreinho/trauma

    Tokio Rust Asynchronous Universal download MAnager

    https://github.com/tokio-rs/tokio



https://elixirforum.com/t/how-hard-would-it-be-to-have-a-static-typing-system-in-elixir/27192

lisp?

racket?

chez scheme? -> fast!



elm language?

no, elm is for the frontend (?)

https://dev.to/mindplay/comment/10kpf

Another reason I'm not personally interested in this language is the lack of static types. For example, Elm is more interesting to me, providing a type system that is so strong that run-time errors don't actually exist.

https://elm-lang.org/examples

does elm support live coding?

reactive functional programming RFP language

https://stackoverflow.com/questions/9448215/tools-to-support-live-coding-as-in-bret-victors-inventing-on-principle-talk





https://old.reddit.com/r/linux/comments/8m2ap2/btfs_a_bittorrent_filesystem_based_on_fuse/

BTFS - A Bittorrent Filesystem Based On FUSE

https://ostechnix.com/btfs-a-bittorrent-filesystem-based-on-fuse/

https://github.com/johang/btfs

https://github.com/acerix/flickmagnet



https://github.com/spacedriveapp/spacedrive

Spacedrive is an open source cross-platform file explorer, powered by a virtual distributed filesystem written in Rust.

Organize files across many devices in one place. From cloud services to offline hard drives, Spacedrive combines the storage capacity and processing power of your devices into one personal distributed cloud, that is both secure and intuitive to use.

For independent creatives, hoarders and those that want to own their digital footprint, Spacedrive provides a free file management experience like no other.

What is a VDFS?

A VDFS (virtual distributed filesystem) is a filesystem designed to work across a variety of storage layers. With a uniform API to manipulate and access content across many devices, VDFS is not restricted to a single machine. It achieves this by maintaining a virtual index of all storage locations, synchronizing the database between clients in realtime. This implementation also uses CAS (Content-addressable storage) to uniquely identify files, while keeping record of logical file paths relative to the storage locations.

The first implementation of a VDFS can be found in this UC Berkeley paper by Haoyuan Li. This paper describes its use for cloud computing, however the underlying concepts can be translated to open consumer software.

Motivation

Many of us have multiple cloud accounts, drives that aren’t backed up and data at risk of loss. We depend on cloud services like Google Photos and iCloud, but are locked in with limited capacity and almost zero interoperability between services and operating systems. Photo albums shouldn’t be stuck in a device ecosystem, or harvested for advertising data. They should be OS agnostic, permanent and personally owned. Data we create is our legacy, that will long outlive us—open source technology is the only way to ensure we retain absolute control over the data that defines our lives, at unlimited scale.



download manager with lua plugins

lua is a popular lightweight scripting language

https://github.com/Y0URD34TH/Project-GLD

  Project GLD is a game library and download manager,
  which supports community made Lua scripts for downloading and searching games.

  written in lua

webscraper in lua

https://github.com/okpanic/lua-spider



emcas?!

  live coding

  declarative

  functional

  https://duckduckgo.com/?q=emacs+web+scraper+download+manager&ia=web

  only the kernel must be stable and fast: async event loop

    rust tokio?

    erlang? faul tolerant

  userspace can be slow: user scripts, plugins, config, state, postprocessing, automation
    web scraper, feed reader, search aggregator, ...

    lua scripts?




scriptable download manager

https://duckduckgo.com/?q=%22scriptable%22+%22download+manager%22&ia=web

https://github.com/sofcat/tdl

  A Simple, Scriptable download manager for the cli. Inspired by DownThemAll. (WIP)

  last commit 2017

https://askubuntu.com/questions/11633/can-you-recommend-a-good-modern-gui-download-manager-wget-wrapper

  http://www.kde.org/applications/internet/kget/

    kget: Downloads from FTP, HTTP(S), torrent sources simultaneously, scriptable, automatic mirror search and more




chez scheme... because fast

https://duckduckgo.com/?q=%22download+manager%22+chez+scheme



scripting languages embeddable in rust 

lua

python

javascript

scheme

static types

https://github.com/dbohdan/embedded-scripting-languages

https://github.com/rhaiscript/rhai

https://www.boringcactus.com/2020/09/16/survey-of-rust-embeddable-scripting-languages.html

mlua (31,454 recent downloads)
rlua (30,877 recent downloads)
duckscript (24,901 recent downloads)
rhai (5,884 recent downloads)
dyon (1,539 recent downloads)
gluon (946 recent downloads)
ketos (497 recent downloads)
rune (495 recent downloads)
ruwren (451 recent downloads)

https://github.com/alilleybrinker/langs-in-rust

https://users.rust-lang.org/t/recommendations-on-an-extension-language/42494

  Be careful with Lua (or Python or JavaScript for that matter).
  These languages can easily undermine the benefits of a strongly typed and type-safe language like Rust.
  You will move cognitive load out to runtime with various runtime exceptions and the like.

https://github.com/rhaiscript/rhai

  dynamic typing

https://github.com/gluon-lang/gluon

  Statically-typed - Static typing makes it easier to write safe and efficient interfaces between gluon and the host application.

  Type inference - Type inference ensures that types rarely have to be written explicitly giving all the benefits of static types with none of the typing.

https://github.com/mun-lang/mun

  Statically typed - Mun resolves types at compilation time instead of at runtime, resulting in immediate feedback when writing code and opening the door for powerful refactoring tools.

  First class hot-reloading - Every aspect of Mun is designed with hot reloading in mind. Hot reloading is the process of changing code and resources of a live application, removing the need to start, stop and recompile an application whenever a function or value is changed.

  very close to rust syntax -> easy to transpile to rust
