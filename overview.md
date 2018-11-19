# "Premise"

## Overview

__*Premise*__ is a collaborative storytelling platform on which people can
  create and explore multiple stories and branching narratives, where each
  story grows from a shared central premise.
  
In the full version, users will be able to create their own 'central premises',
  and make them available for collaborative building. In the MVP release, there
  will be a single, default central premise.

## Target audience

__*Premise*__ primarily targets individuals who enjoy:

* Collaborative worldbuilding and storytelling
* Role-playing games
* Canon-based literature, such as the *Lord of the Rings*, *Harry Potter*,
    and *Star Wars* series.
* Creating and consuming fanfiction
* Exploring the 'butterly effect', where a small change within any given moment
    can lead to very different futures.
* Creative writing exercises

## Structure

The fundamental unit within __*Premise*__ is a __'moment'__ - a user-created
  piece of text no more than 200 characters long. Each individual __moment__
  may be a snippet of dialogue, exposition, descriptive text, etc.
  
__Moments__ are connected sequentially to create a __'story branch'__ or single
  narrative thread within a range of options. Each __story branch__ has
  `first moment` and `last moment` endpoints.

The __'story network'__ is the overall collection of, and relationships between,
  a group of __moments__. Every __moment__ has a single `parent moment`, but may
  have any number of `child moments`. This allows for multiple __story branches__
  evolving from a single `first moment`.

At the core of every __story network__ sits a __'central premise'__ - a set of
  5 __moments__ connected within the __story network__ in a ring.
  __Central premises__ are designed to 'set the stage' for a __story network__,
  and create the core theme around which all _story branches__ in the network
  relate. For example, a __central premise__ might:

* Describe the high-level geography, politics, and time period of a ficitional
    world in which multiple stories will be set.
* Describe a murder scene, from which several genres of mystery will emerge.
* Introduce the relationships between several characters, from which many
    episodes of a soap opera evolve.

A __central premise__ thus creates the central concept or setting from which any
  number of __story branches__ may emerge. The __story branches__, in effect,
  represent parallel universes in which the core concept remains the same, but
  the details and narrative flow are entirely up for grabs. Each subdivision
  along a __story branch__ creates a new parallel universe, such as a murder
  mystery story that continues up to the 'final reveal', and then branches into
  separate branches which implicate each major character!

## Using *Premise*

The core experience in __*Premise*__ involves reading through the moments that
  form the __central premise__, then following/creating different
  __story branches__ that evolve from there. In the full version of the app,
  users would also be able to 'bookmark' specific __moments__, or start at a
  randomly selected, unread __moment__ somewhere within the __story network__.

### Navigating a story network

As the user encounteres each __moment__, they are presented with four primary
  navigational options:
  
* They may __'continue'__, which guides the user down the longest story branch
    that grows from their current position. Defaulting to the longest branch not
    only provides the longest narrative, but helps select for better-developed
    branches, which will tend to yield higher-quality stories, and create a
    richer user journey. In the full version of the app, the method for choosing
    the default __story branch__ would be further optimized.

* They may __'explore'__, which takes the user to a randomly selected __moment__,
    rather than the default branch. This allows users to explore different
    narrative options. In the full version of the app, users would be able to
    select from 'most popular', 'newest', or 'most controversial' branch
    recommendations, in addition to the default 'random' option.

* They may __'create'__, contributing their own __moment__, and starting their
    own story branch for others to follow (and build upon). Users may create
    multiple consecutive __moments__ along a branch, allowing them to build a
    __story branch__ as far as they want.

* They may __'step back'__, moving back to the immediate __parent moment__,
    to either explore a different branch, or to begin creating their own branch.

### Primary user interfaces

#### Reading view

In the __'reading view'__, __moments__ will appear sequentially and append to an
  overall storyline. This view is designed to provide a clean and intuitive
  reading experience with basic navigational controls. It prioritizes immersion
  in a single narrative over awareness of the user's location in the overall
  __story network__.

#### Network view

The __'network view'__ shows how the user's current __moment__ fits within the
  overall __story network__. It shows how the __moment__ traces back to the
  __central premise__, limited information about potential branches going
  forward, and tracing other __story branches__ the user has previously explored.
  Initially, this view will serve primarily for jumping between __moments__
  without having to navigate in a stepwise function. In the full app, this
  view may be used for highlighting popular or bookmarked __moments__, selecting
  and sharing __story branches__ with other users, and highlighting the most
  commonly traveled paths.
  
#### Responsive design

For mobile (and small tablet) users, the __reading view__ will be the primary
  layout, with the ability to toggle to the __network view__ for non-stepwise
  navigation.
  
For desktop (and larger tablet) users, the __network view__ and __reading view__
  will be presented side-by-side.
  
![Mobile reading and network views](https://github.com/sjlutterbie/storychain-dev-notes/blob/overview/img/Reading_Network_Views_2018_11_19.jpg)
![Mobile reading and network views](https://github.com/sjlutterbie/storychain-dev-notes/blob/overview/img/Desktop_Combined_Views_2018_11_19.jpg)