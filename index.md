## Designing The Community Generated Design Language
_To inhabit intricate and completely imagined structures - Intelligence_

![cgen-ui](https://storage.googleapis.com/root-proposal-1246/CGEN/Papers/ACMFAccT2021/ui-proto/cgen-proto-4-purely-components-on.png)

### The Beginning
The team behind the Community Generated Design Language (`cgen-dlang`) has foundations rooted in experiences across information theory, mathematical linguistics, neurobiology, deep reinforcement learning, and cultural evolution/cognitive science.

### The Setting
As students of cognitive science, we view the field of AI on a continuum: 

1. On one end - **Symbolic Systems**
2. On one end - **Connectionism**

The difference between these approaches give rise to various conceptual bridges and perspectives. As a result, we tread carefully, indefinitely and, with great admiration, consider the limits and assumptions of these perspectives and the bridges between them. With that being said, as the human beings behind the `cgen` project, we are also biased in that we want the most straightforward answer to the question:

>_What is the fundamental unit or minimal architecture that gives rise to learning and thus creativity and intelligence in agents of man, machine, animal, plant, culture, and society?_

Through the building of cgen's **framework**, **application**, and **platform**, we aim to answer.

### The Team
As a team of designers, developers, and scientists, we think that such a multidimensional system should be language-agnostic and implementable with any standard programming language like `python` or `R.` Further, the need to design a framework first is to make sure that we could explore both the top-down and bottom-up approaches of generally intelligent systems (GIS). Then, leverage their drawbacks and potentials to make contributions to science and humanity safely

### The Magic
The magic of `cgen` is not only in the machine learning and evolutionary algorithms that underpin the generation of novel products from community participants' input, but the harmony and collaboration between the human participants and the `cgen` system. For `cgen` to be magical, humans must instruct both the imaginations of humans and artificially intelligent systems.

---
> **Paper:** [cgen.dlang: An Evolutionary Approach
> to Design Collaboration](https://storage.googleapis.com/root-proposal-1246/CGEN/Papers/data4good-cgen-dlang.pdf)

![cgen-ui](https://storage.googleapis.com/root-proposal-1246/CGEN/Papers/ACMFAccT2021/ui-proto/cgen-proto-4-plastic-back-shape-on.png)

---
# Introduction
The Community Generated Design Language (`cgen-dlang`, `dlang`, `cgen`, `cd/CD`) is a collaborative design framework developed for small and diverse communities (5 -10 people) who wish to design continually evolving, inclusive, equitable products. Resulting products (or structures) are a product of individually submitted designs and collective decision making. Collective decision making is supported by both the human participants and the evolutionary approach of the cgen framework. To demonstrate, build on, and test the framework, we first highlight how cgen can be used to design products with teams that are composed of various physical impairments or  disabilities. Then, as a final demonstration, we create personas that, through cgen, engage in a community learning space's evolutionary and equitable design. In the end, our results show that creating design products through the cgen framework is possible despite variance in expertise, ability, and role. 

## Software Architecture
`cgen’s` infrastructure relies on a cocktail of programming languages for front-end and back-end specification and implementation.

## Application Architecture
`cgen’s` system architecture. Users interface with the `cgen-dlang` interface to design `structures` (**seed design**) that are functions of the underlying `component library` and associated `grammar`. Users also have the option of `voting()` on other **user-generated structures** and **genetically generated structures**.

## Components  
The structure (system architecture) of `cgen-dlang` is composed of the following components: **component library**, **component grammars**, **voting models**, and an **evolutionary processes**.

### Definitions
* **component library** - _collection of pre-defined `assets`_
* **component grammars** - _set of rules that define
acceptable `operations` on and between `components`
to form `structures`_
* **voting models** - `schema` _outlining the method by which
breeding candidates are selected_

* **evolutionary processes**
    * The `solution space`
    * A `random population` of `genotypes` (possible solutions)
    * Fitness function(s)
    * Virtual `variational operators`: `compare()`, `mutate()`, `cross()`

---
## Install
```python

# Start here
cd cgen_server

# Install dependencies
pip install -r requirements.txt

# And go...
python server.py

# Congifgure front-end
docker run -p 5432:5432 --name cgendlangpostgres -e POSTGRES_PASSWORD=cgendlangpostgres -d postgres

# Navigate to server and install
cd server
npm install

# Create the database structure
node_modules/knex/bin/cli.js migrate:latest

# Generate the first examples
node make_randoms.js

# Generate a cache of image keys for the front page (do it every time you want to update the front page)
node updatecache.js

# And go...
node server.js
```
---
## Use
```python
from cgen.dlang import cgen.example
import cgen.dlang as cgen
import ganbreeder as gan
import tensorflow as tf
import pytorch as torch
import numpy as np

# Generate structure
cgen.Gen_STRUCT(cgen.example.components, ..., cgen.example.operations)

```
---

### Support or Contact
Looking for help or wanting to contribute to the arts and ai? Check out our [documentation](https://github.com/cgen-dlang/cgen-dlang) or [contact team](people.cgen-dlang@gmail.com) and we’ll help you sort it out.
