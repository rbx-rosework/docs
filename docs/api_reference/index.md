---
title: API Reference
---

!!! warning "Under construction"
	This page is under construction - information may be incomplete or missing.

Rosework is split up into many different modules, with each serving a different functionality. Here you can find the API references for each of them:

## Core
This module is the heart of Rosework, and provides the networking and core that most other modules require. It's main feature is the entity[^1] system. It allows subentities[^2] to interact with eachother across the network, especially useful for the State subentity. It also allows for communication between entities.

[Visit the core documentation](core)

## Singleton
The Rosework Singleton module provides the singleton subentity, which is useful for providing service-style functionality

[Visit the singleton documentation](singleton)

## Component

## Tool

## State

## Submodule System
The Rosework [submodule system](sms) is designed to minimize the amount of code put into a single file by splitting all of that code up into many different files. 

You can do this using Luau's built in ``require()`` function, but it would eliminate the ability to easily use Rosework's API, or other (sub)modules from within that submodule.

[Visit the submodule system documentation](sms)

----

[^1]: An entity is the base of everything in Rosework. An entity should only contain one feature, and may use as many subentities as it likes.

[^2]: A subentity is anything that lives inside a normal Rosework entity created by Rosework/Core