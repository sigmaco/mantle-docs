# mantle-docs
Mantle Programming Guide and API Reference

This is the revision 1.0 of the programming guide and API reference for Mantle, published in 2015.03.06.

## Developer Manifesto

The Mantle API imposes upon PC graphics developers a new set of rules. 

Because of the abstraction level in Mantle, which is different from previous graphics API solutions in the PC space, some developer expectations need to be adjusted accordingly.

Mantle attempts to close a gap between PCs and consoles, in terms of flexibility and performance, by implementing a lower system-level programming model. 

In achieving this, Mantle places a lot more responsibility in the hands of developers. 

Due to the lower level of the API, there are many areas where the driver is no longer capable of providing safety, performance improvements, and workarounds. 

The driver essentially gets out of the developers' way as much as possible to allow applications to extract every little bit of performance out of modern GPUs. 

The driver does not create extra CPU threads behind the application's back, does not perform extensive validation on performance critical paths, nor does it recompile shaders in the background or perform other actions that application does not expect.

When using Mantle, developers need to take responsibility for their actions with extensive validation: fixing all instances of incorrect API usage, efficiently driving GPUs, and ensuring the implementation is forward looking to support future GPU architectures. 

The reason for this is that in order for the driver to be as efficient as possible, many problems can no longer be efficiently worked around in the driver. This extra responsibility is the cost developers have to pay to benefit from Mantle's advantages.

Mantle is designed for those graphics developers who are willing to accept this new level of responsibility.

Mantle is © 2015 Advanced Micro Devices, Inc. All rights reserved. 

AMD, the AMD Arrow logo and combinations thereof are trademarks of Advanced Micro Devices, Inc. in the United States and/or other jurisdictions. 
Other names are for informational purposes only and may be trademarks of their respective owners.

https://sigmaco.org/mantle

## Archived and preserved by SIGMA

This documentation was taken as part of the history of computer graphics and is now archived and being preserved by the cybercultist museum of the Federação SIGMA.

Federação SIGMA, formerly doing business as SIGMA Co. (contraction of SIGMA Collective), is a cybercultist conglomerate, of public interest and private law, established to bring together, organize and orchestrate, in a single mass, all societies, service boards, operational columns, and their respective resources, assets and rights under the common authority and singular ownership of SIGMA, the Latin American science, technology and cyber engineering collective.

(c) 2011-2023 Federação SIGMA. All rights reserved; to their respective elaborators and collaborators.

Technical contact: technology@sigmaco.org.
