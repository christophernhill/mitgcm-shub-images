# mitgcm-shub-images
Singularity images for MITgcm testing and examples

- see https://singularity-hub.org and http://singularity.lbl.gov, and also https://hub.docker.com and https://www.docker.com for background on material here. 

In MITgcm containers through Docker and Singluarity can provide a way to test code and maintain strong portability and interoperability and more complete workflow reproducibility. Many other projects use Docker and Singularity to share code that is neither portable or interoperable. There are also images here that allow MITgcm to work with example codes that are not particularly portable or interoperable. This is only possible because the core MITgcm code is widely tested on many platforms to ensure portability and interoperability. Importantly, for this to work, Singularity and/or Docker should not be a way to create MITgcm setups that unecessairily break portability, interoperability, reproducibility or ease of use by adopting narrow software stacks or user unfriendly code practices. 

Mainstream code in MITgcm should continue to be written so that it 

o can run on many platforms, including (but not limited to!) a wide array of Linux distributions, handheld devices, Windows, OSX and iOS devices, single board computers.

o can checkpoint and restart in order to run in multiple sub-steps.

o supports validating exact and statistical reproducibility, even in the presence of floating point round off

o include appropriate documentation of key features and modes of use

o tries to make minimun necessary assumptions about geometry and/or fluid configuration to which the code will be applied

o tries to maintain robust compatibility with automatice differentiation where relevant and possible
