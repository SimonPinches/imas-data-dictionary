# IMAS Data Dictionary

The Data Dictionary is the implementation of the Data Model of ITER's
Integrated Modelling & Analysis Suite (IMAS). It describes the
structuring and naming of data (as a set of Interface Data Structures
or IDSs) being used for both simulated and experimental data in a
machine agnostic manner.



## Installation
It's possible to install the Data Dictionary within a Python environment.

> Prerequisite : A Python interpreter and the Saxon library should be preinstalled

```sh
git clone git@github.com:iterorganization/imas-data-dictionary.git
cd imas-data-dictionary
pip install . [--user]
```

After the install, you will get a directory with the version/tag information 
prefixed with `dd_` e.g. `dd_4.0.0`. It has an `include` directory with a few
XML files (`IDSdef.xml` is the main source of information for the definition 
of IDSs and `*_indentifier.xml` are listing common identifiers) and a `share` 
directory with html documentation.

### Documentation (Sphinx)

If you want to generate sphinx documentation then you need `Python` 
and `Saxon`. For generating the IDS Migration guide you need `IMASPy` installed.
You can generate and install this documentation with the following steps:

```bash
pip install -r docs/requirements.txt
python generate_docs.py
pip install .
```

### `idsinfo` tool

The installation also provides a small utility script in Python which can be 
used from the command line to obtain some information from the installed 
Data Dictionary. Type `idsinfo -h` for more info on this tool's options.



## Collaboration

As it is generic and machine agnostic by design, the IMAS Data Model,
and by extension its implementation as the Data Dictionary, have the
potential to serve as a data standard for the fusion community. As
such, it benefits from the wide involvement of specialists and active
users and developers in the various areas being described. If you want
to contribute to the improvement of the Data Dictionary, either as a
developer, a specific system/area specialist or an occasional user
providing feedback, please see the [contributing guidelines](CONTRIBUTING.md).



## Legal
Copyright 2012-2024, ITER Organization, Route de Vinon-sur-Verdon, CS 90 046, 
13067 St-Paul-lez-Durance Cedex, France.

This repository contains data schemas and software that are subject to different 
licenses:

* The data schemas are licensed under the Creative Commons 
Attribution-Noderivatives 4.0 International License (CC-BY-ND 4.0) which permits 
use and distribution as long as appropriate credit is given to the original source, 
but does not permit adaptations, as the main goal of these schemas is to serve as 
a standard for the community. 
Details can be found in [LICENSE-CC-BY-ND](LICENSE-CC-BY-ND).

* The software is licensed under the LGPLv3 License which allows for extensive 
freedom in using, modifying, and distributing it, provided that the license terms 
are met. 
Details can be found in [LICENSE-LGPL](LICENSE-LGPL).

