---
layout: single
title: Program
permalink: /program/
include_subs: true
---

# Thursday, 2025-07-03

| Time  | Activity |
|-------|----------|
| 08:30 | Registration Opens |
| 09:00 | Welcome and Opening |
| 09:15 | [Keynote 1](#keynote-1) |
| 10:15 | Coffee Break |
| 10:30 | [Technical Session 1](#technical-session-1) |
| 12:00 | Lunch Break |
| 13:30 | [Technical Session 2](#technical-session-2) |
| 15:00 | Coffee Break |
| 15:20 | Information Regarding the [Social Event](#social-event--dinner) |
| 15:45 | Meetup for the [Social Event](#social-event--dinner) |
| 18:30 | [Dinner](#social-event--dinner) at 1965m Altitude |


# Friday, 2025-07-04

| Time  | Activity |
|-------|----------|
| 09:00 | [Keynote 2](#keynote-2) |
| 10:00 | Coffee Break |
| 10:30 | [Technical Session 3](#technical-session-3) |
| 12:00 | Lunch Break |
| 13:30 | [Technical Session 4](#technical-session-4) |
| 14:30 | Closing Statement |
| 15:00 | Coffee Break and Farewell |

---

## Keynote 1

### Towards more Flexible and Dynamic HPC Software Stacks for the Post-Exascale Era
[Prof. Dr. Martin Schulz](https://www.ce.cit.tum.de/caps/mitarbeiter/martin-schulz)
{% include abstract.html 
text="High-Performance Computing (HPC) is at an
inflection point in its evolution. General-purpose architectures approach
limits in terms of speed and power/energy, requiring the development of
specialized architectures to deliver accelerated performance. At the same time,
data movement has been identified as a main culprit of energy waste, pushing
hardware designers towards a tighter integration of the different technologies.
The result is a trend to integrated systems, which offer great opportunities in
terms of power/performance tradeoffs, but also lead to challenges on the
software side. They require new dynamic concepts in operating systems and
programming models, all the way to system-wide resource management.

However, such approaches lead to substantial challenges on the software side:
accelerators must be efficiently utilized and/or explicitly enabled or disabled,
workloads must be balanced across potentially different technologies, energy
consumption must be balanced with the expected performance improvements, and
large accelerator appliances must be explicitly scheduled. Solving these
challenges requires us to look at new approaches on the system software side and
ultimately breaking with long-lived HPC paradigms, including rigid resource
allocation or single tenancy per node. This will open a new level of flexibility
that can enable the efficient utilization of systems with customization or
specialization." %}

## Technical Session 1

**PHI: a modern C++ library for parallel pattern composition**  
Santiago Veigas Ramírez, Daniel Martínez Davies and José Daniel García Sánchez
{% include abstract.html 
text="This paper presents the design of PHI, a modern C++ library that allows for the
composable expression of parallel computation patterns. Building upon the
principles of GrPPI, PHI introduces a range-like interface that enables for
declarative composition of parallel patterns by means of a pipe-like syntax that
better aligns with contemporary C++ idioms. Additionally, PHI's architecture
aims to separate pattern composition from its execution, allowing for
backend-agnostic implementations, and the potential to integrate various
execution models." %}

**Enabling Pinning Strategies for Stream Processing Applications on Multicores**  
Lorenzo Bindi, Salvatore D'Amico, Gabriele Mencagli and Massimo Torquati
{% include abstract.html 
text="Data stream processing (DSP) applications consist of
data-flow graphs of operators that process data streams. These operators run as
dedicated threads, either in parallel or concurrently, on computing platforms
with multi-core CPUs. The decision of where to run threads of parallel programs,
specifically which CPU core of the underlying architecture to use, is known as
thread pinning, and it can significantly affect application's throughput. For
DSP applications, finding an efficient pinning can be challenging as it depends
on information about the data-flow structure, operator types, and communication
patterns. Although thread pinning is a low-level optimization available in
several parallel programming frameworks, DSP frameworks typically do not allow
users to configure thread pinning, leaving the decision to the Operating System.
This paper extends the WindFlow library, and its FastFlow-based parallel runtime
system, to expose thread pinning mechanisms through an usable API. The
effectiveness of this approach is demonstrated through extensive evaluations of
four applications, using six custom pinning strategies on a high-end server." %}

**Mneme: A Parallel Preprocessing Framework for Large Tabular Datasets**  
Argiris Sofotasios, Dimitris Metaxakis and Panagiotis Hadjidoukas
{% include abstract.html 
text="The rapid expansion of Machine Learning (ML)
applications, especially within its subfield of Deep Learning (DL), has created
an increasing demand for efficient preprocessing of large tabular datasets that
surpass the available memory capacity. This paper introduces a parallel
framework, developed as a Python library, designed to efficiently preprocess
large-scale tabular datasets for training deep neural networks. The library
supports various data transformations, including normalization, categorical
encoding and missing value imputation, leveraging parallel computing and
chunk-based processing to handle massive datasets efficiently. By distributing
preprocessing tasks across multiple cores and facilitating the parallel loading
and processing of data chunks without altering the original data file, the
proposed library significantly reduces the time required for data preparation,
which often represents a critical bottleneck in modern ML pipelines.
Experimental evaluation demonstrates substantial performance gains over
conventional sequential approaches and state-of-the-art solutions. Furthermore,
the library integrates seamlessly with widely adopted deep learning frameworks,
providing a scalable and flexible High-Performance Computing (HPC) tool for data
preprocessing in contemporary ML workflows." %}

## Technical Session 2

**SkePU-Streaming: Distributed Pipelining of Portable Data-Parallel Skeleton
Computations for the Heterogeneous Edge-Cloud Continuum**  
August Svensson, Fabio Crugnola, August Ernstsson, Sajad Khosravi, Sebastian Litzinger and Christoph
Kessler
{% include abstract.html 
text="We present SkePU-Streaming, a two-layer
high-level programming framework for specifying complex pipelines composed of
portable multi-backend stream processing tasks, each expressed by algorithmic
skeletons or user-provided implementations, and its deployment toolchain for
distributed heterogeneous parallel systems. Pipeline tasks can have multiple
variants to more flexibly exploit the resources of heterogeneous nodes; the
convenient expression of multi-variant tasks is achieved by integrating the
high-level C++ based skeleton programming framework SkePU with its multiple
backends as the main method for portable programming of the stream-processing
tasks. Concretely, SkePU-Streaming adds an abstraction layer for pipeline
workflow specifications atop SkePU-based task specifications, and extends the
SkePU data-container API with stream access operators for use within SkePU and
other C++ task code. We present the SkePU-Streaming design and its
implementation in a deployment framework for distributed heterogeneous parallel
systems, and report on early experimental evaluation results." %}

**A Zero-Overhead Transpiler-Based Python Frontend for the Skeleton Programming
Framework SkePU**  
Axel Hammarberg, August Ernstsson and Christoph Kessler
{% include abstract.html
text="We extend the skeleton programming framework SkePU with an all-new
Python-based interface and frontend with zero run-time overhead. Skeleton
programming is a powerful, high-abstraction-level approach to programming of
parallel and heterogeneous computer systems. SkePU is a skeleton programming
framework consisting of a C++ template header library as well as a Clang-based
source-to-source translator. Until now, SkePU programs have been written
exclusively as C++ programs, utilizing the power of C++ compiler infrastructure
for multi-backend support and mature optimization, together ensuring performance
portability. However, C++ is now challenged as a high-level programming
language, and novice users are often uncomfortable using it. We therefore aim to
increase the usability of SkePU by extending the framework with a Python-like
interface utilizing a Python-to-C++ source-to-source translator. The new
frontend is based on the existing Shed Skin translator, which as part of this
work has been extended with support for variadic template code generation and
other advanced C++-features utilized by SkePU. The resulting toolchain enables
whole SkePU programs to be written in a restricted, implicitly statically-typed
subset of Python syntax. We evaluate the compile-time overhead of Python-to-C++
transpilation. We also demonstrate the absence of run-time overhead of our
solution by comparing the execution times of SkePU programs written in both C++
and Python, and evaluate the run-time performance against related work." %}

**Towards Extreme Scalability of Stencil Applications with Parallel Skeletons**  
David Díez, Sergio Alonso Pascual and Arturo Gonzalez-Escribano
{% include abstract.html
text="The pre- and exascale computational systems require new programming tools
and solutions to develop and deploy applications with extreme scalability. Most
of them include heterogeneous devices and accelerators. Programming for these
platforms generally requires mixing computations programmed using low level or
portability models with partition and communication mechanisms across nodes and
devices to overlap computation and communication efficiently. A relevant class
of scientific applications that require this kind of solution to obtain a high
degree of scalability are the ISL (Iterative Loop Stencil) applications. EPSILOD
is a parallel skeleton for ISL applications targeting heterogeneous distributed
systems. In this work, we present an extension of EPSILOD that enables a new
range of applications using generic data types, a new domain-specific language
for optimized kernel integration, and a new synchronization and communication
scheme to increase scalability in Tier-0 computing facilities. We test the new
solutions using examples, including simple 2D stencils and a 3D
Lattice-Boltzmann stencil application. We present an experimental study
comparing EPSILOD with Muesli, a state-of-the-art skeleton solution for stencil
applications, scaling up to 1024 GPUs distributed in 256 nodes. The results show
that EPSILOD obtains better performance results, with high degrees of strong and
weak scalability." %}

## Keynote 2

### Types as a path from abstract to performance?
[Prof. Dr. Gabriele Keller](https://www.uu.nl/staff/GKKeller)
{% include abstract.html 
text="Even though the declarative semantics of purely functional languages offers
clear advantages in the space of parallel computing, their high level of
abstraction makes it challenging to achieve performance which is close to
hand-optimised low-level code. On the other hand, it also requires a significant
time investment from programmers to acquire the expertise to write performant
code for multi-core and especially GPU architectures. Even for experts, writing
and debugging these programs is time-consuming, and the resulting code is in
general not portable across different architectures.  

In this presentation, I will talk about how we use the advanced type features of
the functional language Haskell to provide an embedded language for multi-core
and GPU programming. The language allows programmers to write architecture
independent programs, whose performance is, in many cases, close to, or
sometimes faster than hand-written code.  We employ these type features to
improve the reliability of the compiler, provide a smooth embedding and stronger
static checks for the user, eliminating many runtime errors." %}

## Technical Session 3

**High-level Programming of Vulkan-based GPUs through OpenMP**  
Ilias K. Kasmeridis and Vassilios V. Dimakopoulos
{% include abstract.html
text="Modern applications often involve complex, structured, or data-parallel
computations on large datasets. Traditionally, GPUs have served as the primary
accelerators for such tasks, mostly through compute-focused models such as CUDA
and OpenCL. Vulkan is another recent cross-platform API, widely adopted for both
high-performance graphics and compute. Such models require lower-level
programming, as developers have to be aware of architectural details; this is
not easily accomplished given the dramatic rise in hardware heterogeneity. It
has thus become increasingly desirable to adopt higher-level models that
abstract away the low-level hardware and API details, and simplify GPU
programming. In this paper we present a full-fledged OpenMP translator and
runtime offloading infrastructure that targets the Vulkan Compute pipeline.
While previous works usually focus on OpenCL or CUDA, this is the first time an
OpenMP compiler targets Vulkan shaders. As such, apart from the support for
off-the-shelf NVIDIA and AMD GPUs, we are the first to provide OpenMP support
for mobile and embedded GPUs, such as VideoCore GPUs. The proposed translator,
which is based on an open-source compilation framework, receives standard OpenMP
code and converts it to tunable Vulkan shaders. Our approach preserves the
simplicity of higher-level programming, while still achieving high performance,
as demonstrated by our experimental results." %}

**A High-level API for End-to-end Data Compression in Multi-GPU Cluster
Applications**  
Gabriel Mitterrutzner, Peter Thoman and Philipp Gschwandtner
{% include abstract.html
text="The increasing complexity of high-performance computing (HPC) systems,
particularly those utilizing a multi-GPU cluster architecture, presents
significant challenges for developers. Low-level, vendor-specific application
programming interfaces (APIs) often require deep technical knowledge,
complicating maintenance and reducing performance portability. This complexity
is exacerbated when large data sizes or bandwidth requirements necessitate data
compression. Integrating such end-to-end compression into existing codebases
dealing with distributed memory multi-GPU clusters is often labor-intensive and
error-prone, particularly when flexibility in the choice of compression
algorithm and implementation is desired.

In this work, we propose a high-level, user-friendly end-to-end data compression
API integrated into the Celerity runtime system, built on the SYCL programming
model. By abstracting the complexities of integrating various compression
algorithms, we aim to enhance data transfer and storage efficiency, without a
large cost in development complexity. Our API supports multiple compression
types and memory layouts, enabling developers to leverage compression without
extensive modifications to their existing codebases. We evaluate this API and
its prototype implementation in various benchmarks, demonstrating its
effectiveness in reducing storage and bandwidth requirements, while maintaining
high performance." %}

**SymTensor: Symbolic and Adaptive Tensor Partitioning by Unified Parallelism
for Deep Learning**  
Hongxing Wang, Chong Li, Zhengdao Yu and Serge Petiton
{% include abstract.html
text="The rapid expansion of deep learning models in scale and structural
diversity has made distributed training essential. Designing efficient
parallelization strategies requires balancing computation, communication, and
memory. However, existing methods struggle to coordinate multiple
parallelization strategies across different model components and to adapt to
changing models. This paper proposes SymTensor, a strategy generation method
based on a principled tensor-level cost model without relying on predefined
rules. SymTensor unifies different forms of parallelism into a single system and
formulates a symbolic model to jointly analyze computation, communication, and
memory costs. It employs an adaptive tensor partitioning algorithm to minimize
total cost. Our proposal adapts to changes such as model architectures, operator
types, and input shapes. Our experiments on representative foundation models
demonstrate that SymTensor-generated strategies achieve up to 221% of the
training performance compared to those generated by the state-of-the-art
Megatron-LM. Our tensor-based symbolic-cost-driven solution provides strong
efficiency, adaptability, and practicality over large-scale distributed
training." %}

## Technical Session 4

**East of Eden: Parallel Functional Programming in Idris**  
Christopher Brown and Adam Barwell
{% include abstract.html
text="There have been various different attempts to introduce parallel
programming models into functional languages, from very implicit approaches,
such as the par and pseq model exhibited by GpH, to semi-explicit process models
exhibited by the Haskell implementation, Eden, to very explicit actor-based
models that use message passing and explicit process creation, such as Erlang.
Implicit vs. explicit parallel models introduce important tradeoffs to
programmers. Explicit models give more control over the parallelism, but require
much more low-level management (and often more expertise from the programmer);
implicit approaches give less control over the parallelism (and therefore often
require less parallel expertise) but offer more reasoning opportunities.
However, to date, there has been little exploration to introduce implicit
parallelism approaches to an emerging class of dependently typed programming
languages.

Dependently-typed programming languages, such as Idris, Agda and Coq, allow
programmers to encode specifications of their programs as specialised types that
depend on values. This value dependence means that the types express logical
relations and the programs provide proof obligations that the relations hold.
With the exception of pi-par, an extension to Idris with explicit process
creation and message passing, there are little to no parallel dependently-typed
languages that offer implicit parallel models to the programmer.

In this paper we introduce a semi-implicit programming model, similar to Eden
for Haskell, by extending Idris with a dependently-typed process abstraction.
This semi-implicit process model means that processes can be explicitly created,
but low-level details, such as communication, synchronisation and scheduling is
abstracted away by the runtime. Furthermore, our process model is enhanced by
making use of dependent-types to allow some of the parallel behaviour to be
exposed to the programmer at the type level. In turn, this enables further
typing abstractions that describe common parallel patterns and skeletons.

In this paper we make the following contributions:

- We introduce a novel semi-implicit depedently-typed parallel process language
  as an extension to Idris.
- We provide common data and task parallel patterns that are built on our
  process model, and expose these to the programmer.
- We describe a backend for achieving our parallelism using Erlang.
- We demonstrate our process language on a number of examples for both data and
  task parallelism on a 28-core machine." %}

---

# Social Event & Dinner

The social event will take place on the first day of the symposium, July 3, 2025.
We will meet right in front of the Ágnes-Heller-Haus at 15:45, and board public transport to the base station of the [Patscherkofelbahn](https://www.patscherkofelbahn.at/en), a cable car that will take us to the Patscherkofel mountain at 1965m altitude.
There, we will enjoy a dinner at "Das Kofel", with a stunning view over Innsbruck and the surrounding mountains.

![Das Kofel]({{ site.baseurl }}/assets/images/dinner_kofel.jpg)
