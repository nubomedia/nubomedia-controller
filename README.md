# NUBOMEDIA Controller

This project is part of NUBOMEDIA project: [nubomedia.eu][NUBOMEDIA]

[![][NUBOMEDIA Logo]][NUBOMEDIA]

Copyright © 2016 [NUBOMEDIA]. Licensed under [Apache 2.0 License].

The NUBOMEDIA Controller (nubomedia-controller) is an integration of different projects providing together the PaaS functionalities for Multimedia Applications.

## Component List

The NUBOMEDIA Controller contains the following components: 

 * NUBOMEDIA Platform as a Service
 * NUBOMEDIA Marketplace
 * Open Baton NFV Orchestrator
 * Open Baton Generic VNFM 
 * Kurento VNFM

Please refer to the NUBOMEDIA Architecture deliverable [NUBOMEDIA D2.4.2] for more details about the interaction between different components. Here you can find the architecture diagram.


[![][NUBOMEDIA Architecture]][NUBOMEDIA]

## How to install

### Requirements 

In order to install the nubomedia-controller, you need to have running: 

 * OpenStack: providing the IaaS functionalities and exposing VIM interfaces towards Open Baton NFVO
 * OpenShift: providing the PaaS functionalities and exposing the PaaS interface towards the nubomedia-paas manager

### Install the nubomedia-controller binary version

In order to install the nubomedia-controller you need to refer to the autonomous installer

### Install the nubomedia-controller using the source code version

In order to install the nubomedia-controller using the source code version, you need to follow the steps provided here. 
1) Checkout this repository and move into the folder. 

```bash
git clone --recursive https://github.com/nubomedia/nubomedia-controller.git
cd nubomedia-controller
```

2) create required folders under opt

```bash
sudo mkdir /opt/openbaton
sudo mkdir /opt/nubomedia
```

3) Copy or link these folders under opt in such way: 
```bash
sudo cp -r NFVO /opt/openbaton/
sudo cp -r generic-vnfm /opt/openbaton
sudo cp -r marketplace /opt/nubomedia
sudo cp -r nubomedia-msvfnm /opt/nubomedia
sudo cp -r nubomedia-paas /opt/nubomedia
```

4) compile the source code of each component and start the configuration process. You can refer to each individual project git repository for more details about the installation procedure.
We suggest you follow the following order while installing the tools:

 * NFVO
 * generic-vnfm
 * nubomedia-msvnfm
 * marketplace
 * nubomedia-paas


# What is NUBOMEDIA

This project is part of [NUBOMEDIA], which is an open source cloud Platform as a
Service (PaaS) which makes possible to integrate Real Time Communications (RTC)
and multimedia through advanced media processing capabilities. The aim of
NUBOMEDIA is to democratize multimedia technologies helping all developers to
include advanced multimedia capabilities into their Web and smartphone
applications in a simple, direct and fast manner. To accomplish that objective,
NUBOMEDIA provides a set of APIs that try to abstract all the low level details
of service deployment, management, and exploitation allowing applications to
transparently scale and adapt to the required load while preserving QoS
guarantees.

# Documentation

The [NUBOMEDIA] project provides detailed documentation including tutorials,
installation and [Development Guide].

# Source

Source code for other NUBOMEDIA projects can be found in the [GitHub NUBOMEDIA
Group].


# News

Follow us on Twitter @[NUBOMEDIA Twitter].

# Issue tracker

Issues and bug reports should be posted to [GitHub Issues].

# Licensing and distribution

Software associated to NUBOMEDIA is provided as open source under GNU Library or
"Lesser" General Public License, version 2.1 (LGPL-2.1). Please check the
specific terms and conditions linked to this open source license at
http://opensource.org/licenses/LGPL-2.1. Please note that software derived as a
result of modifying the source code of NUBOMEDIA software in order to fix a bug
or incorporate enhancements is considered a derivative work of the product.
Software that merely uses or aggregates (i.e. links to) an otherwise unmodified
version of existing software is not considered a derivative work.

# Contribution policy

You can contribute to the NUBOMEDIA community through bug-reports, bug-fixes,
new code or new documentation. For contributing to the NUBOMEDIA community,
drop a post to the [NUBOMEDIA Public Mailing List] providing full information
about your contribution and its value. In your contributions, you must comply
with the following guidelines

* You must specify the specific contents of your contribution either through a
  detailed bug description, through a pull-request or through a patch.
* You must specify the licensing restrictions of the code you contribute.
* For newly created code to be incorporated in the NUBOMEDIA code-base, you
  must accept NUBOMEDIA to own the code copyright, so that its open source
  nature is guaranteed.
* You must justify appropriately the need and value of your contribution. The
  NUBOMEDIA project has no obligations in relation to accepting contributions
  from third parties.
* The NUBOMEDIA project leaders have the right of asking for further
  explanations, tests or validations of any code contributed to the community
  before it being incorporated into the NUBOMEDIA code-base. You must be ready
  to addressing all these kind of concerns before having your code approved.

# Support

The NUBOMEDIA community provides support through the [NUBOMEDIA Public Mailing List].

[Apache 2.0 License]: https://www.apache.org/licenses/LICENSE-2.0.txt
[Development Guide]: http://nubomedia.readthedocs.org/
[GitHub Issues]: https://github.com/tub-nubomedia/marketplace/issues
[GitHub NUBOMEDIA Group]: https://github.com/nubomedia
[NUBOMEDIA Architecture]: http://www.nubomedia.eu/sites/default/files/images/nubomedia-arch-600.png
[NUBOMEDIA D2.4.2]:http://www.nubomedia.eu/sites/default/deliverables/WP2/D2.4.2_Architecture_R6_V2_26-01-2016_FINAL-PC.pdf
[NUBOMEDIA Logo]: http://www.nubomedia.eu/sites/default/files/nubomedia_logo-small.png
[NUBOMEDIA Twitter]: https://twitter.com/nubomedia
[NUBOMEDIA Public Mailing list]: https://groups.google.com/forum/#!forum/nubomedia-dev
[NUBOMEDIA]: http://www.nubomedia.eu
