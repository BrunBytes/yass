# Notes On Implementation:

This document stores all my musings as the project progresses. To-Do tools are a joke so this is a lot better

## RESEARCH NOTES

I think Bjarne had it wrong with *Zero Cost Abstractions* - it's a pipe dream. It's not concievable to achieve. Function pointers are the devil that will sink us all. Algebraic data types are what he should've focused on instead, AKA *Tagged Unions*. However I have alternative proposal I'd like to explore in this project, namely the principle of *Zero Cost Expressions*. This is the intention that we have a program backed up and enforced in correctness through a rich type system, that does not sacrifice runtime performance. The zero cost is transferred between both the programmer and the system itself. This is superior to both the OOP of modern software design, as well as not relying on the fairly untouched academic theory of the 1960s that powers most performant games that is an abosolute nightmare to use. It all sounds fairly abstract right now, but I hope this project will showcase what I'm talking about and convince us there's a way to be fast and beautiful. 

## PRE_ALPHA

For us to be considerd Pre-Alpha we need these systems to be functional

- [] Intial libraries decided
    - [] Macroquad for Render/Platform functionality for now?
    - [] Networking Library
    - [] lua integration library
- [] Basic game flow satisfied
    - [] As a client I can connect to a local server
    - [] As a client I can locomote in the world
    - [] Very rudimentary UI system
    - [] Lua scripting for server conditions


## ALPHA

For us to be considered alpha we need these systems to be functional

- [] Sound system
    - [] Proper occlusion/range based sound system
- [] Object templates
    - [] Allow for objects to be placed in the world
- [] Map maker
    - [] Allow for maps to be loaded and saved
- [] Core gameplay systems implemented
    - [] Atmos
    - [] Power
    - [] Doors
    - [] Access
    - [] Health (advanced, not basic system)
    - [] Crafting
    - [] Recipes
    - [] Inventory
    - [] Interactions
    - [] Death/Ghosting

Polish at this stage can be super minimal, just need all the systems present.

## BETA

For us to be considered Beta, we need these systems to be functional

- [] GUIs operational (this includes in-game and outside)
- [] Full lobby flow
- [] Client connections (no direct point of failure like wizden. You need to be given IP and a valid key to join. Servers can ban per Key/IP)
- [] Session persistence (servers can store data for managing bans/access etc. Clients can store characters and servers they've added)
- [] Antags and rolls working.
- [] Evac
- [] Departments functional, but not fleshed out.


## SHIPPABLE

For us to be considered shippable, we need these systems to be functional

- [] All departments fleshed out
  - [] Medical
  - [] Science
  - [] Command
  - [] Sec
  - [] Cargo
  - [] Engineering
  - [] Service
- [] Antagonist Support
  - [] Syndicate
  - [] Traitor
  - [] Thief
  - [] Zombies
  - [] Revs
  - [] Nukies
- [] Final online systems
  - [] Support packed assets properly
  - [] multiple engine versioning support
- [] Maps ported over (TBD which ones)

## RELEASED

Need to think about this, likely adding many minor antags as well as the more complex major ones. At this point most of the work should be in lua 
