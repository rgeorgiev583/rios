# Rios

**Rios** is an interface-oriented operating system written in the Rust programming language.
It follows the operating system specification called **AIOS**.

## What is an interface-oriented operating system?
It means that the main design principle of the operating system is to expose its API through well-defined object-like interfaces that fit into a neat hierarchy.
This means that the purpose of all syscalls exposed by the OS will be to create and maintain the nodes of the hierarchy.
This idea is not dissimilar to the API filesystem approach spearheaded by the innovative *Plan 9* operating system created by the Bell Labs team (by some of the people who created Unix).

## So does this mean that basically this is an object-oriented operating system?
Yes and no.
It can be said that this OS is object-oriented because it exposes interfaces to things which, well, are actually objects.
However, the focus of the whole thing is not how the objects are actually implemented (their fields, etc.) but how they are accessed (i.e. the interfaces they provide).

## Why deviate from previous approaches to OS development?
Because I want to design the system in a radically different way which I have not yet seen implemented (as far as I have researched).
I want to create a system where things which are achieved in contemporary operating systems using a multitude of different syscalls with different purposes to be achievable simply through interacting with the object-like interface that the OS provides.
