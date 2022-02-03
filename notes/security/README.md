## Notes about software systems security

Practicing **Security by Design** implies thinking about security at each stage while desigining a system to meet functional and non-functional requirements. 

### STRIDE
The S.T.R.I.D.E. is a security threat model.

> The STRIDE approach to threat modeling was invented by Loren Kohnfelder and Praerit Garg (Kohnfelder, 1999). This framework and mnemonic was designed to help people developing software identify the types of attacks that software tends to experience.
> 
> -- from "Threat Modeling: Designing for Security" by Adam Shostack

- **Spoofing** happens when an actor (user or system) claims they are someone else or something else
- **Tampering** happens when data (or system configuration) is altered in an unauthorised way due to some (external) interference 
- **Repudiation** happens when an actor (user or system) claims they have not performed an action (even though they in reality did)
- **Denial of Service** happens when a system becomes unavailable or its performance degrades
- **Information Disclosure** happens when an actor (user or system) leaks some information
- **Elevation of Priviledge** happens when an actor (user or system) gains capabilities they are not supposed to have
