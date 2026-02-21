
+++

title = "MICRO-MACRO COMPUTATIONAL MODELS: THEORY, APPLICATIONS AND EMERGENT PROPERTIES"
description = "Module 2"
outputs = ["Reveal"]
aliases = [
    "/guide/"
]

+++


# MICRO-MACRO COMPUTATIONAL MODELS: THEORY, APPLICATIONS AND EMERGENT PROPERTIES
## Module 2

## [Danilo Pianini](mailto:danilo.pianini@unibo.it) - {{% today %}}

---

# Part 1: Nature-inspired systems and emergence

---

{{< slide background-image="img/monza.png" >}}

---

<video width="120%" height="120%" autoplay controls loop><source data-src="https://danysk.github.io/Slides-2019-OYM/video/stampede.mp4" type="video/webm" /></video>

---

## Context: large-scale open systems

Typical setting:
- Networked systems with many participants
- Heterogeneous devices (capabilities, energy, sensors/actuators)
- Partial knowledge, unreliable communication
- Dynamic topology (mobility, churn)
- Situatedness: space and time matter
- No stable coordinator

---

## Engineering problem: Collective Adaptive Systems (CASs)

We want systems that are:
- Distributed and scalable
- Adaptive to changes (environment, participants, goals)
- Robust to failures and uncertainty
- Maintainable and evolvable over time

Key question:
> How do we engineer global behavior from local components?

---

## The “obvious” approach: centralize

Pipeline:
1. Gather data to a central point
2. Compute decisions centrally
3. Push actions back to devices

Typical issues:
- Single point of failure
- Scalability bottleneck
- High latency (worse at high density)
- Privacy and governance concerns
- Inefficient use of network/computation at the edge

---

## So… decentralize?

{{% multicol %}}
{{% col %}}
* No single coordinator
* Local interactions only
* No global state
* No single control loop
* Local interactions must produce coherent global behavior

> How do we design these systems reliably?

{{% /col %}}
{{% col %}}
<video width="50%" height="100%" autoplay controls loop><source data-src="video/mantis-hornet.mp4" type="video/webm" /></video>
{{% /col %}}
{{% /multicol %}}

---

## What “no coordinator” implies

Constraints that shape the engineering:
- No global state
- No single control loop
- Local interactions only (limited range, limited bandwidth)
- Faults are normal (dropouts, delays, partitions)
- The system must still behave coherently at the macro level

---

## Nature inspiration (general)

Bio-inspired design as engineering transfer:
- Identify a function that nature performs well
- Abstract the mechanism (not the biological details)
- Re-implement under engineering constraints
- Validate against measurable requirements

---

{{< slide background-image="https://danysk.github.io/Slides-2019-OYM/img/spider-man.jpg" >}}

---

{{< slide background-image="https://upload.wikimedia.org/wikipedia/commons/1/1b/Gecko_leopard.jpg" >}}


---

{{< youtube id="uEYcY7WfDTY?start=7">}}

---

{{< youtube id="uhfXbSSrabw" autostart="true">}}

---

## Gecko-inspired dry adhesion

{{% multicol %}}
{{% col %}}
![Gecko Pad design](https://danysk.github.io/Slides-2019-OYM/img/geckopad.jpg)

- Function-driven design (adhesion without glue)
- Mechanism abstraction (micro-/nano-structures to increase contact)
- Engineering outcome (reusable, scalable dry adhesives)
{{% /col %}}
{{% col %}}

![Gecko Pad design](https://danysk.github.io/Slides-2019-OYM/img/biomimicry-gecko-climging-pads.jpg)
{{% /col %}}
{{% /multicol %}}

---

{{< slide background-image="https://danysk.github.io/Slides-2019-OYM/img/500nozomi.jpg" >}}

---

## Shinkansen series 500

- Tunnel boom: sonic boom-like noise when exiting tunnels at high speed
- Caused by buildup and rapid release of pressure waves
- Constraints: need to maintain high speed and passenger comfort

> What can we learn from nature to solve this?

---

{{< slide background-image="https://upload.wikimedia.org/wikipedia/commons/2/29/Common_kingfisher_in_flight.jpg" >}}

---

{{< youtube id="veQ2ilQrzMU?start=20">}}

---

{{< slide background-image="https://danysk.github.io/Slides-2019-OYM/img/700series.jpg" >}}

---

## Shinkansen series 700

- Solution: geometry inspired by kingfisher beak
- Outcome: reduced noise, improved aerodynamics

---

## Back to CAS: what nature can teach

For collective adaptive systems we look for:
- Leaderless coordination
- Local sensing + local communication
- Feedback loops and self-regulation
- Robustness through redundancy and adaptation

Core idea:
> Local rules can produce macroscopic structure.

---

## Self-organising systems

One way to tackle these challenges is through systems that *self-organise*.

* *Self-organisation* is a process in which a system spontaneously organizes itself into a structured state without external control.
* It is a **bottom-up** process in which local interactions among components lead to the **emergence** of global patterns or structures.
* Self-organisation is often observed in *natural systems*, such as biological organisms, ecosystems, and social systems.
* It can also be applied to artificial systems, such as robotics, distributed computing, and complex networks.

---

<div id="div1" style="width: 720px; float: left; overflow: hidden;">
  <img src="https://danysk.github.io/Slides-2019-OYM/img/ants.jpg" style="position:relative; width: 100%; height: 100%; border: 0; margin:auto; overflow: hidden;"/>
</div>
<div id="div2" style="width: 720px; float: left; overflow: hidden;">
  <img src="https://danysk.github.io/Slides-2019-OYM/img/termites.jpg" style="position:relative; width: 100%; height: 100%; border: 0; margin:auto; overflow: hidden;"/>
</div>
<div id="div3" style="width: 720px; float: left; overflow: hidden;">
  <img src="https://danysk.github.io/Slides-2019-OYM/img/firefly.jpg" style="position:relative; width: 100%; height: 100%; border: 0; margin:auto; overflow: hidden;"/>
</div>
<div id="div4" style="width: 720px; float: left; overflow: hidden;">
  <img src="https://danysk.github.io/Slides-2019-OYM/img/ecosystem.jpg" style="position:relative; width: 100%; height: 100%; border: 0; margin:auto; overflow: hidden;"/>
</div>

---

<iframe
width="1920" height="950"
src="https://www.youtube.com/embed/ZHpu7ngQxwE?si=YPGltxUIp5QtcOlV"
autoplay="true"
title="YouTube video player"
frameborder="0"
allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
referrerpolicy="strict-origin-when-cross-origin"
allowfullscreen>
</iframe>

---

<iframe
src="https://www.netlogoweb.org/launch#https://www.netlogoweb.org/assets/modelslib/Sample%20Models/Biology/Ants.nlogo"
style="position: relative; top: 0; left: 0; width: 100%; height: 28em;">
</iframe>

---

# Part 2: Simulation paradigms and modeling choices

---

## Why simulation for *CAS*

Simulation is the practical way to:
- test hypotheses on *collective behavior* at scale
- explore *what-if scenarios* safely (no harm, no disruption)
- study *scalability limits* and *failure modes* before deployment
- build **repeatable** and comparable experiments

---

## Why simulation for *CAS*

A *model* is a simplified representation of reality:
- keep what matters for the *question* we are asking
- abstract away what is irrelevant or infeasible to reproduce

We simulate when the real process:
- takes too long
- is hard to replicate in controlled conditions
- is dangerous to replicate
- is beyond our technical capacity

---

## Simulation in the engineering loop

For collective systems, simulation is used for:
- *prototyping* (quick feedback on system-level behavior)
- *testing* (including regression tests)
- *debugging* (replaying scenarios across runs)
- *profiling* (performance and scalability assessment)

---

## Simulation semantics

**Modeling choices affect outcomes.**

Key dimensions:
- *discrete vs continuous time*
- *time-driven vs event-driven*
- *synchronous vs asynchronous scheduling*
- *deterministic vs stochastic evolution*
- **reproducibility** and control of randomness

---

## *Time-driven* vs *event-driven*

*Time-driven* (ticks):
- time advances in fixed steps
- system state is updated at each tick
- “simultaneity” is enforced within a tick

*Event-driven* (*discrete-event simulation*):
- time advances to the next scheduled event
- events are processed one by one
- if two events share a timestamp, an execution order still exists (**and may matter**)

---

## *Synchronous* vs *asynchronous* scheduling

*Synchronous*:
- all agents update together (typical in tick-based ABM tools)
- easy to reason about, but introduces **artificial simultaneity**

*Asynchronous*:
- agents update at different times
- closer to many real distributed settings
- ordering effects become **part of the model**

---

## *Stochasticity* and **reproducibility**

In computer simulation, **reproducibility requires**:
- controlling random *seeds* explicitly
- understanding that parallelism can introduce *non-determinism*
- making ordering assumptions explicit (especially in *discrete-event simulation*)

Practical rule:
- every result should specify: *model*, *parameters*, *seeds*, and execution configuration

---

## Monte Carlo framing

Two extremes:
- *exhaustive exploration* (often infeasible)
- *sampling-based exploration* (*Monte Carlo*)

*Monte Carlo method*:
- randomly explore part of the space
- repeat many times
- aggregate results into estimates

---

## Simulation as a *Monte Carlo* run

Simulation is often one step in a pipeline:

1. choose parameters (or sample them)
2. run multiple *seeds* per configuration
3. compute *summary statistics* (mean/variance/quantiles)
4. estimate *uncertainty* (confidence intervals)
5. compare alternatives (*sensitivity* / *ablation* / *robustness*)

---

## Batch thinking

A single run answers: *“what happened once”*  
A Monte Carlo experiment answers: **“what tends to happen”**

Good practice:
- separate *model specification* from *experiment design*
- plan what you *measure* before running batches
- keep outputs minimal but sufficient for analysis

---

## Why *Alchemist*

Alchemist is a general-purpose simulator for *networked systems*:
- nodes in an *environment*
- *neighborhood relations* (possibly dynamic)
- *reactions* as the unit of behavior
- supports *situated* scenarios (space matters)
- supports *maps* and *floor plans* (image-based)
- used as an *external simulator* for aggregate programming prototyping and debugging

---

## Alchemist (video)

<video loop playsinline autoplay muted style="max-width: 900px; display: inline-block;">
  <source src="https://alchemistsimulator.github.io/home-animation.mp4" type="video/mp4">
  If your browser supported the video tag, there would be a nice video.
</video>

---

## Alchemist conceptual model

Core concepts:
- *Nodes* (devices / agents / compartments)
- *Environment* (space + constraints)
- *Reactions* (what can happen, and when)
- *Time* (typically *discrete-event*, with customizable time distributions)

Practical implication:
- changing the *time model* or *scheduling policy* can change **emergent outcomes**

---

## Deploying devices and configuring connections

Deployment answers: *“where are the devices?”*  
Typical strategies:
- random placement
- regular grids and perturbed grids
- scenario-specific placement (clusters, hotspots)
- mobility models (moving nodes over time)

---

## Deploying devices and configuring connections

Connectivity answers: *“who can talk to whom?”*  
Typical ingredients:
- *neighborhood definition* (e.g., range-based, metric-based, constrained by environment)
- *network dynamics* (links appear/disappear as nodes move or conditions change)
- communication assumptions (latency/loss models, if included)

Engineering note:
- **“neighborhood” is part of the model, not an implementation detail**

---

## Dynamics and timing

Two families of dynamics:
- state changes triggered by *time-driven* rounds (ticks)
- state changes triggered by *events* with time distributions

In *discrete-event* settings:
- events are ordered even at equal timestamps (**ordering can bias outcomes**)
- non-Markovian events are possible (custom time distributions)

---

## Environments: *obstacles* and *maps*

Environment is **not** just a background:
- it constrains motion and interaction
- it shapes connectivity (blocked paths, partitions, funnels)
- it changes what “distance” means (*Euclidean* vs *walkable routes*)

---

## Obstacles/maps change the network

Effects you must account for:
- two devices can be close in *Euclidean space* but disconnected in practice
- barriers can create *communities* and *bottlenecks*
- routing distance may be a better metric than geometric distance in built environments

---

## Loading spatial data

Common approaches:
- floor plans / maps as images (*obstacles encoded in pixels*)
- environment-aware metrics (e.g., *route-based distances*)
- scenario composition: same program, different environments

Key point:
- environment selection can **dominate** the observed macro behavior


---

## What we build next (hook to Lecture 3)

Next: bottom-up emergence in simulation
- implement local interaction rules and observe macro patterns
- build canonical building blocks (e.g., diffusion/gradient-like spreading)
- study limitations: fragility, tuning sensitivity, reusability and composability issues

---

### Lecture 2 (2h) — Simulation paradigms and modeling choices

**Time budget (120’)**

* 15’ Why simulation for CAS: testing hypotheses, safety, scalability
* 30’ Simulation semantics: discrete vs continuous time; time-driven vs event-driven; synchronous vs asynchronous; stochasticity/reproducibility
* 20’ Monte Carlo framing: simulation as one run inside an exploration/estimation pipeline (parameter sweeps, uncertainty, confidence)
* 25’ Alchemist positioning: why it as reference simulator; conceptual model (nodes, environment, reactions, time)
* 25’ Deploying devices + configuring connections: neighborhoods, network models, dynamics
* 25’ Environments: obstacles/maps; loading spatial data; effects on connectivity and behavior
* 15’ Wrap-up: typical modeling pitfalls + what will be built next (hook to Lecture 3)

---

## Engineering self-organisation

* Self-organisation is **very hard to engineer**
* The system properties are built **bottom-up** from **local interactions**
* Even worse, even when a self-organizing system has been built and verified,
  it is extremely hard to **reuse** it in a different context

### Where is the *engineering*?

There are properties that we cannot renounce:
* *Top-down design*
* *Modularity*
* *Reusability*
* *Composability*
* *Scalability*
* *Maintainability*

---

### Lecture 3 (2h) — Bottom-up emergence and its limitations

**Time budget (120’)**

* 10’ Goal and framing: bottom-up emergence as an engineering technique; where it breaks
* 20’ Coordination as a first-class tool: interaction through shared abstractions vs direct messaging
* 20’ Tuple spaces / computing in the medium: intuition + compositionality via multiple spaces/centers
* 25’ Worked example: distributed dodgeball (or equivalent) as a bottom-up emergent system
* 20’ Distributed information spreading: gradient as a recurring “macro pattern”
* 15’ Slow-rising problem (Beal): why it happens; bottom-up fixes/patches
* 10’ Limits: reusability/modularity issues; transition motivation to aggregate computing (hook to Lecture 4)

---

### Lecture 4 (2h) — Engineering emergence with aggregate computing

**Time budget (120’)**

* 10’ Motivation: higher abstraction, modular reuse of collective behavior; contrast with Lecture 3 limits
* 15’ Core idea: fields over space/time; language-based approach to collective behavior
* 15’ Core constructs: neighboring, evolution, domain segmentation (what each enables)
* 10’ Core semantics: exchange vs share (why this matters for reasoning and composition)
* 10’ Short history: aggregate programming languages (positioning, not a survey)
* 25’ Collektive model + building blocks: gradient, collection, leader election (concept + how you use them)
* 20’ Patterns: gradient, channel, network centre, bull’s eye (guided mini-designs / mapping to blocks)
* 15’ Advanced examples: VMC, Kiel channel, robot coordination; synthesis and closure


---

# Headers

# H1
## H2
### H3
#### H4

---

# Text

normal text

`inline code`

*italic*

**bold**

**_emphasized_**

*__emphasized alternative__*

~~strikethrough~~

[link](http://www.google.com)

---

# Lists and enums

1. First ordered list item
1. Another item
    * Unordered sub-list.
    * with two items
        * another sublist
            1. With a sub-enum
            1. yay!
1. Actual numbers don't matter, just that it's a number
  1. Ordered sub-list
1. And another item.

---

# Inline images

![Alternative text](https://upload.wikimedia.org/wikipedia/commons/6/6c/Scavolino_innevata.jpg)

---

## Fallback to shortcodes for resizing

Autoresize specifying

* `max-w` (percent of parent element width) and/or `max-h` (percent of viewport height) as max sizes , and
* `width` and/or `height` as *exact* sizes (as percent of viewport size)

{{< figure src="https://upload.wikimedia.org/wikipedia/commons/6/6c/Scavolino_innevata.jpg" height="20">}}

---

## Multi-column slide

{{% multicol %}}{{% col %}}
Column 1
{{% /col %}}{{% col %}}
Column 2
{{% /col %}}{{% /multicol %}}

{{% multicol %}}
{{% col class="col-8" %}}
Larger columns using bootstrap
{{% /col %}}
{{% col %}}
[Link to bootstrap grid system](https://getbootstrap.com/docs/4.0/layout/grid/)
{{% /col %}}
{{% /multicol %}}


---

## Tick and Cross

* {{% tick %}} This is something good
* {{% cross %}} This is something bad

---

## Chart.js

{{< chart >}}
{
    type: 'bar',
    data: {
        labels: ['Red', 'Blue', 'Yellow', 'Green', 'Purple', 'Orange'],
        datasets: [{
            label: 'Bar Chart',
            data: [12, 19, 18, 16, 13, 14],
            backgroundColor: [
                'rgba(255, 99, 132, 0.2)',
                'rgba(54, 162, 235, 0.2)',
                'rgba(255, 206, 86, 0.2)',
                'rgba(75, 192, 192, 0.2)',
                'rgba(153, 102, 255, 0.2)',
                'rgba(255, 159, 64, 0.2)'
            ],
            borderColor: [
                'rgba(255, 99, 132, 1)',
                'rgba(54, 162, 235, 1)',
                'rgba(255, 206, 86, 1)',
                'rgba(75, 192, 192, 1)',
                'rgba(153, 102, 255, 1)',
                'rgba(255, 159, 64, 1)'
            ],
            borderWidth: 1
        }]
    },
    options: {
        maintainAspectRatio: false,
        scales: {
            yAxes: [{
                ticks: {
                    beginAtZero: true
                }
            }]
        }
    }
}
{{< /chart >}}

---

## FontAwesome

<i class="fa-solid fa-mug-hot"></i>
<i class="fa-solid fa-lemon"></i>
<i class="fa-solid fa-flask"></i>
<i class="fa-solid fa-apple-whole"></i>
<i class="fa-solid fa-bacon"></i>
<i class="fa-solid fa-beer-mug-empty"></i>
<i class="fa-solid fa-pepper-hot"></i>

---

## Bootstrap 1

<div class="card w-100" >
  <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/e/e9/View_of_Cesena_from_the_Abbey.jpg/1920px-View_of_Cesena_from_the_Abbey.jpg" class="card-img-top" alt="...">
  <div class="card-body">
    <h5 class="card-title">Card title</h5>
    <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
    <a href="#" class="btn btn-primary">Go somewhere</a>
  </div>
</div>

---

## Bootstrap 2

<button type="button" class="btn btn-primary">Primary</button>
<button type="button" class="btn btn-secondary">Secondary</button>
<button type="button" class="btn btn-success">Success</button>
<button type="button" class="btn btn-danger">Danger</button>
<button type="button" class="btn btn-warning">Warning</button>
<button type="button" class="btn btn-info">Info</button>
<button type="button" class="btn btn-light">Light</button>
<button type="button" class="btn btn-dark">Dark</button>

<button type="button" class="btn btn-link">Link</button>

---

## Low res, plain markdown

![](https://upload.wikimedia.org/wikipedia/commons/thumb/6/6c/Scavolino_innevata.jpg/260px-Scavolino_innevata.jpg)

---

## Hi res, plain markdown

![](https://upload.wikimedia.org/wikipedia/commons/6/6c/Scavolino_innevata.jpg)

---

{{< slide background-image="https://upload.wikimedia.org/wikipedia/commons/6/6c/Scavolino_innevata.jpg" >}}

# Large images as background
## (May affect printing)

---


{{< slide background-video="https://github.com/DanySK/slides-2024-acsos-imageonomics/raw/master/content/nonnadir.mkv" background-video-loop="true" background-video-muted="true" background-opacity="0.95">}}

# Video background

---

# $$\LaTeX{}$$


Inline equations like $E=mc^2$

$$\frac{n!}{k!(n-k)!} = \binom{n}{k}$$

---

# Code snippets


```kotlin
val x = pippo
```

```go
package main

import "fmt"

func main() {
    fmt.Println("Hello world!")
}
```

---

# Tables

Colons can be used to align columns.

| Tables        | Are           | Cool  |
| ------------- |:-------------:| -----:|
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| zebra stripes | are neat      |    $1 |

There must be at least 3 dashes separating each header cell.
The outer pipes (|) are optional, and you don't need to make the
raw Markdown line up prettily. You can also use inline Markdown.

---

# Quotes

> Multiple
> lines
> of
> a
> single
> quote
> get
> joined

> Very long one liners of Markdown text automatically get broken into a multiline quotation, which is then rendered in the slides.

---

# Fragments

* {{< frag c="pluto" >}}
* {{< frag c="pluto" >}}
* {{< frag c="pluto" >}}

---

# Stacking images with Fragments
{{% multicol %}}
{{% col %}}
<p class="fragment" data-fragment-index="0">Pippo</p>
<p class="fragment" data-fragment-index="1">Pluto</p>
<p class="fragment" data-fragment-index="2">Paperino</p>
{{%/ col %}}

{{% col %}}
<div class="r-stack">
  <img
    class="fragment current-visible"
    data-fragment-index="0"
    src="https://www.topolino.it/wp-content/uploads/2019/12/pippointera.png"
    width="450"
    height="300"
  />
  <img
    class="fragment current-visible"
    data-fragment-index="1"
    src="https://www.topolino.it/wp-content/uploads/2019/12/plutointera.png"
    width="300"
    height="450"
  />
  <img
    class="fragment current-visible"
    data-fragment-index="2"
    src="https://it.wikifur.com/w/images/thumb/6/6f/Donald_Duck.png/362px-Donald_Duck.png"
    width="400"
    height="400"
  />
</div>
{{%/ col %}}

{{%/ multicol %}}


---

# Graphs via Gravizo

{{< gravizo "Example Gravizo graph" >}}
  digraph G {
    aize ="4,4";
    main [shape=box];
    main -> parse [weight=8];
    parse -> execute;
    main -> init [style=dotted];
    main -> cleanup;
    execute -> { make_string; printf}
    init -> make_string;
    edge [color=red];
    main -> printf [style=bold,label="100 times"];
    make_string [label="make a string"];
    node [shape=box,style=filled,color=".7 .3 1.0"];
    execute -> compare;
  }
{{< /gravizo >}}

---

# Graphs via mermaid.js

```mermaid
classDiagram
  Class01 <|-- AveryLongClass : Coosssl
  Class03 *-- Class04
  Class05 o-- Class06
  Class07 .. Class08
  Class09 --> C2 : Where am i?
  Class09 --* C3
  Class09 --|> Class07
  Class07 : equals()
  Class07 : Object[] elementData
  Class01 : size()
  Class01 : int chimp
  Class01 : int gorillasaaaaaaaaaaaaaaaaaaaaaa
  Class08 <--> C2: Cool label
```

---


# Graphs via mermaid.js with options

```mermaid
%%{init: {'theme':'default', 'themeVariables': { 'fontSize': '.34em', 'fontFamily': 'verdana' }}}%%
classDiagram
  Class01 <|-- AveryLongClass : Coosssl
  Class03 *-- Class04
  Class05 o-- Class06
  Class07 .. Class08
  Class09 --> C2 : Where am i?
  Class09 --* C3
  Class09 --|> Class07
  Class07 : equals()
  Class07 : Object[] elementData
  Class01 : size()
  Class01 : int chimp
  Class01 : int gorillasaaaaaaaaaaaaaaaaaaaaaa
  Class08 <--> C2: Cool label
```


---
# Graphs via mermaid.js 2

```mermaid
graph TD
  SL([fa:fa-user second level]) --> L[solution]
  L -- solution email --> db[(mysql)]
  db --> X[automatic]
  X --> CM([fa:fa-users first level])
  db -- Email --> c([customer support]);
```

---

# Graphs via mermaid.js 3

```mermaid
gitGraph
  commit id: "Initialize project"
  commit id: "Make some changes"
  branch develop
  checkout develop
  commit
  commit
  checkout main
  merge develop
  commit
  commit
```

---

# Keystrokes

<kbd>Ctrl</kbd> + <kbd>Alt</kbd> + <kbd>Del</kbd>

---

# QR code

{{% qrcode data="https://www.google.com" %}}

---

# Import shared slides

<!-- write-here "shared-slides/devops/devops-intro.md" -->
<!-- end-write -->
