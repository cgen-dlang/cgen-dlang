# cgen-dlang: Community Generated Design Language

[![ForTheBadge powered-by-electricity](http://ForTheBadge.com/images/badges/powered-by-electricity.svg)](http://ForTheBadge.com)

[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/commit-activity)
[![Website shields.io](https://img.shields.io/website-up-down-green-red/http/shields.io.svg)](http://shields.io/)
[![PyPI license](https://img.shields.io/pypi/l/ansicolortags.svg)](https://pypi.python.org/pypi/ansicolortags/)

_An Evolutionary Approach to Design Collaboration_

---

# Introduction

[`cgen-dlang`]() is a collaborative design system developed for small communities (5 – 50 people) who want to generate a collection of the team specific  computer aided structures, which are likely to be optimal reflections of a team’s aesthetic values: These visual structures capture the full transmission history of aesthetics and are used to form design language systems. 

## Software Architecture

`cgen-dlang` infrastructure relies on a cocktail of programming languages for front-end and back-end specification and implementation.

## Application Architecture

`cgen-dlang` system architecture. Users interface with the `cgen-dlang` interface to design `structures` (**seed design**) that are functions of the underlying `component library` and associated `grammar`. Users also have the option of `voting()` on other **user-generated structures** and **genetically generated structures**.

## Components 

The structure (system architecture) of `cgen-dlang` is composed of the following components: **component library**, **component grammars**, **voting models**, and **evolutionary processes**.

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
Looking for help or wanting to contribute to the arts and ai? Check out our [documentation](https://github.com/cgen-dlang/cgen-dlang) or [contact team](people.cgen.dlang@gmail.com) and we’ll help you sort it out.

---

[![ForTheBadge built-by-developers](http://ForTheBadge.com/images/badges/built-by-developers.svg)](https://GitHub.com/Naereen/)
[![ForTheBadge built-with-love](http://ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/Naereen/)
