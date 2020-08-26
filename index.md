---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: home
---

# The 7th Workshop on Formal Reasoning in Distributed Algorithms

Dates: September 3rd to September 5th 2020

Online workshop from 6pm to 8pm CET

The workshop is organized as part of [QONFEST 2020](http://qonfest2020.conf.tuwien.ac.at/), also hosting [CONCUR 2020](https://concur2020.forsyte.at/).

Registration is required at <https://qonfest2020.github.io/registration.html>.
Workshop-only registration costs 5 Euros until August 13th and then 8 Euros.

## News

* August 25th 2020:
  * Program update: [Murdoch James Gabbay](http://gabbay.org.uk/) will talk
    about a mathematical analysis of the (E)UTxO blockchain architecture on
    Friday September 4th.
* August 6th 2020:
  * [Marco Carbone](https://www.itu.dk/people/maca/), a leading expert on session types, will give an introduction
    to session types on Friday September 4th.
  * Tentative program posted
  * The schedule has been shifted by half an hour, for a start at 6pm, in order
    to avoid conflict with other talks at QONFEST.

## Tentative Program (to be confirmed)

* Thursday September 3rd
  - 6pm to 6:40pm: [Yotam Feldman](https://www.cs.tau.ac.il/research/yotam.feldman/), Tel Aviv University
    <details>
    <summary>Inferring Inductive Invariants from Phase Structures (click to expand the abstract)</summary>
      <br>
      <p>
      Infinite-state systems such as distributed protocols are challenging to verify using interactive theorem provers or automatic verification tools. Of these techniques, deductive verification is highly expressive but requires the user to annotate the system with inductive invariants. To relieve the user from this labor-intensive and challenging task, invariant inference aims to find inductive invariants automatically. Unfortunately, when applied to infinite-state systems such as distributed protocols, existing inference techniques often diverge, which greatly limits their applicability.
      </p>

      <p>
      This work proposes user-guided invariant inference based on phase invariants, which capture the different logical phases of the protocol. The user conveys their intuition by specifying a phase structure, an automaton with edges labeled by program transitions; the tool automatically infers assertions that hold in the automaton's states, resulting in a full safety proof. The additional structure of phases provides guidance to the inference procedure about how to find an invariant.
      </p>

      <p>
      Our results show that user guidance by phase structures facilitates successful inference beyond the state of the art. We find that phase structures are pleasantly well matched to the intuitive reasoning routinely used by domain experts to understand why distributed protocols are correct, so that providing a phase structure reuses this existing intuition.
      </p>

    </details>

  * 6:40pm to 7:20pm: Lacramioara Astefanoaei, [Nomadic Labs](https://nomadic-labs.com/)
    <details>
    <summary>Using Maude for modeling consensus algorithms in blockchains (click to expand the abstract)</summary>

      <br>
      <p>
      Recently, formal methods are increasingly being used in the blockchain
      space to gain confidence in the underlying consensus algorithms. In this
      talk, i would like to share with you some early experiments showing how
      Maude strategy language can effectively help to better understand
      consensus logic.
      </p>
    </details>
  * 7:20pm to 8pm: [Mohsen Lesani](https://www.cs.ucr.edu/~lesani/), University of California, Riverside
    <details>
    <summary>Replication Coordination Analysis and Synthesis, The Journey from Convergence to Integrity and recency.</summary>

      <br>
      <p>
      Distributed system replication is widely used as a means of fault-tolerance and scalability. Traditional strong consistency maintains the same total order of operations across replicas. This total order is the immediate source of multiple desirable consistency properties: integrity, convergence and recency. However, maintaining the total order has proven to inhibit availability and performance. Weaker notions exhibit responsiveness and scalability; however, they forfeit the total order and hence its favorable properties. The project Hamsan revives these properties with as little coordination as possible. It presents a tool that, given a sequential class with the declaration of its integrity and recency requirements, automatically synthesizes a correct-by-construction replicated class that simultaneously guarantees the three properties. The approach is based on novel sufficient conditions for integrity, convergence and recency that require certain orders between conflicting and dependent operations, and constrain pending operations. To decide the validity of coordination-avoidance conditions, the tool applies automatic solvers to analyze both the given class statically and the operations dynamically. It then reduces coordination to classical minimization problems and instantiates novel parametric coordination protocols. The experiments show that the synthesized replicated objects are significantly more responsive than the strongly consistent baseline.
      </p>

    </details>
* Friday September 4th
  * 6pm to 6:40pm: [Damien Zufferey](https://dzufferey.github.io/), Max Planck Institute for Software Systems (MPI-SWS)
    <details>
    <summary>Implementing Communication-Closed Rounds: Toward an Efficient and General Solution (click to expand the abstract)</summary>

      <br>
      <p>
      Implementing fault-tolerant distributed algorithms (FTDA) is difficult and error-prone. Verifying the implementation of one of these algorithms is even harder. The PSync project started as a way of simplifying the verification of FTDA by implementing a round model (Heard-Of model). While PSync simplifies an FTDA implementation, the abstraction has a performance cost and the runtime fixes the fault-model (partially synchronous networks.)
      </p>
      <p>
      In the first part of this talk, I will describe how PSync is implemented and the solutions we found to offer decent performances. However, some common optimizations are the combination of the communication pattern of the algorithm and the fault model. Such optimization are not possible in PSync as the runtime has to work for all possible algorithms. In the second part, I will discuss how we took the lessons from PSync to extend the model to give the user more control over the round abstraction. Our goal is to have a configurable runtime system for the Heard-Of model that can be deployed with a variety of settings, including Byzantine faults, and enable optimization which depends on the interplay of the FTDA, the fault model, and the deployment conditions.
      </p>
      <p>
      This is based on ongoing work with Cezara Dragoi and Josef Widder.
      </p>
    </details>
  * 6:40pm to 7:20pm: [Marco Carbone](https://www.itu.dk/people/maca/), IT University of Copenhagen
    <details>
    <summary>Introduction to session types</summary>
    </details>
  * 7:20pm to 8pm: [Murdoch James Gabbay](http://gabbay.org.uk/), Heriot-Watt University
    <details>
    <summary>A mathematical analysis of the (E)UTxO blockchain architecture (click to expand the abstract)</summary>

      <br>
      <p>
      The UTxO (unspent transaction output) model is the underlying data structure of Bitcoin, which has also been extended to the Extended UTxO model.  I will present a novel mathematical model of (E)UTxO based on some very simple type equations which — for me at least — make it easier to see what is structurally going on.  Time permitting, I will show how to derive from these equations a model of blockchains as algebras of partially-ordered partial monoids with channels.  These ideas exist as a full journal paper and a Haskell reference implementation.
      </p>

      <p>
      <a href="https://arxiv.org/abs/2003.14271">A conference paper</a>, <a href="https://arxiv.org/abs/2007.12404">a journal paper (submitted)</a>, and <a href="https://github.com/bellissimogiorno/nominal/blob/master/src/Language/Nominal/Examples/IdealisedEUTxO.hs">Haskell code</a> are available now.
      </p>
    </details>
* Saturday September 5th
  * 6pm to 6:40pm: Balasubramanian A.R., Technical University of Munich
    <details>
    <summary>Complexity of Verification and Synthesis of Threshold Automata (click to expand the abstract)</summary>

      <br>
      <p>
      Threshold automata are a formalism for modeling and analyzing
      fault-tolerant distributed algorithms, recently introduced by Konnov,
      Veith, and Widder, describing protocols executed by a fixed but
      arbitrary number of processes.
      </p>
      <p>
      We conduct the first systematic study of the complexity of verification
      and synthesis problems for threshold automata.
      We prove that the coverability, reachability, safety, and liveness
      problems are NP-complete, and that the bounded synthesis problem is
      Σₚ² complete.
      </p>
      <p>
      A key to our results is a novel characterization of the reachability
      relation of a threshold automaton as an existential Presburger formula.
      The characterization also leads to novel verification and synthesis
      algorithms. We report on an implementation and provide experimental
      results.
      </p>

    </details>
  * 6:40pm to 7:20pm: [Borzoo Bonakdarpour](http://web.cs.iastate.edu/~borzoo/), Michigan State University
    <details>
    <summary>Parametrized Synthesis of Distributed Self-stabilizing Protocols (click to see the abstract)</summary>

      <br>
      <p>
      Program synthesis is often called the "holy grail" of computer science, as it enables users to refrain from error-prone software development process and focus on only analyzing the intended behavior of the system. Thus, program synthesis exhibits its power in automatic generation of intricate and complex parts of a system as well as in repetitive programming tasks, and bringing the power of programming to the average computer user who may not possess sophisticated programming skills. A particular area where program synthesis can play a central role is in distributed systems due to their inherent complex nature. This talk will present our recent results and breakthroughs in synthesizing parameterized distributed self-stabilizing algorithms.
      </p>

    </details>
  * 7:20pm to 8pm: [James R. Wilcox](https://jamesrwilcox.com/), [Certora](https://certora.com/)
    <details>
    <summary>The mypyvy intermediate language for symbolic transition systems (click to see the abstract)</summary>

      <br>
      <p>
      mypyvy is a straightforward modeling language for representing transition systems in first-order logic that supports verification and invariant inference. Once a transition system has been expressed in mypyvy, users can state safety properties of the system and prove them by giving a sufficiently strong inductive invariant. However, mypyvy's primary purpose is not to support manual verification, but rather to support research on invariant inference algorithms that automatically construct an inductive invariant given the safety property. We have implemented several state-of-the-art invariant inference algorithms in mypyvy and used them to automatically verify challenging examples from the distributed systems literature, such as sophisticated variants of Paxos. This talk will be a tutorial introduction to this style of verification and invariant inference in mypyvy and will include live demos.
      </p>
    </details>


## Summary of the workshop

Distributed algorithms is an active research field; their applications range
from Internet applications over cloud computing to safety-critical control
systems. Whereas many applications are of critical importance, the correctness
of distributed algorithms is usually based on very subtle mathematical
arguments. Consequently, one easily can make mistakes with hand-written proofs,
which reduces the trust in the correctness of these systems.

In the last decades, formal methods were proven to be useful for the
verification of many hardware and software systems. For distributed algorithms,
the application of formal methods was limited: formal methods have been used
for finding bugs in distributed algorithms, and to a much smaller extent formal
methods were used in computer-aided verification of simple distributed
algorithms. However, to verify more involved distributed algorithms, one cannot
easily apply existing verification tools. To be eventually able to do this, an
interdisciplinary effort from the concerned fields of formal methods, logic in
computer science, and distributed algorithm theory is required.

The topics of interest for the FRIDA workshop include the following topics, as
they apply to distributed algorithms and systems:

* formal modeling
* model checking
* interactive theorem proving
* parameterized model checking
* integration of different verification techniques
* benchmarking
* synthesis
* run-time verification
* testing
* invariant inference


## Organizers

* [Marijana Lazić](https://www7.in.tum.de/~lazic/) [(email)](mailto:lazic@in.tum.de)
* [Giuliano Losa](https://www.losa.fr/) [(email)](mailto:giuliano@galois.com)

## Previous editions

Starting a productive dialogue between distributed algorithms and verification
communities was the goal of a successful [Dagstuhl Seminar “Formal Verification
of Distributed Algorithms”](https://www.dagstuhl.de/en/program/calendar/semhp/?semnr=13141)
which was held in April 2013. During this seminar,
the participants agreed that a series of workshops should be held in order to
strengthen the community that does research on these issues.

The [1st workshop on Formal Reasoning in Distributed
Algorithms](https://easychair.org/smart-program/VSL2014/FRIDA-index.html)
took place in Vienna as part of the Vienna Summer of Logic’14 and Federated
Logic Conference’14.
The [2nd FRIDA workshop](http://discotec2015.inria.fr/workshops/frida-2015/)
took place in Grenoble as part of FORTE’15.
The [3rd FRIDA workshop](https://forsyte.at/events/frida2016/)
was organized in Marrakech as part of NETYS’16.
The [4th FRIDA workshop](https://forsyte.at/events/frida2017/)
took place in Vienna as part of DISC 2017.
The [5th FRIDA workshop](https://forsyte.at/events/frida2018/) was
co-located with CAV 2018, which was held as part of the
Federated Logic Conference (FLoC).
The [6th workshop](https://team.inria.fr/veridis/events/frida2019/) was
co-located with DISC 2019 in Budapest, Hungary.
