# StoryChain: Dev Notes

StoryChain is a collaborative storytelling platform where users can add 'storyLinks'
to story chains, follow the stories that evolve from the storyLinks they create, and
uncover how different story chains interconnect.

## Definitions & details

**storyLink** - A single unit of narrative, ast most 200 characters in length.

  * Each `storyLink` has one `parent storyLink`.
  * Each `storyLink` may have zero or more `child storyLinks`.

**Story Chain** - A ordered set of `storyLinks` that share a parent-child lineage
  from a `first parent storyLink` to a `last child storyLink`.

**Story Network** - A hierarchical set of `storyLinks`, containing multiple
  branching `Story Chains`, connected by a single `first parent storyLink`.
  
  * Each user will have one or more `Story Networks`, which will be limited by
      their access `[read|unread|hidden]` to each individual `storyLink`.

**Saga** - A full set of interconnected `Story Chains`.

  * Each `Saga` is defined by a title, summary statement, and its `Starting Ring`.
  
**Starting Ring** - A set of 5 or more `storyLinks` that create a looping
  `storyChain`.

  * Using a `Starting Ring` ensures that every link in a Saga has a single parent.
  * Because a ring can ONLY be created as a `Starting Ring`, it ensures that users
      can clearly identify when they've discovered the full origin of the `Saga`.

## User stories

### Pre-login:

As a site visitor, I should be able to:

* Learn about StoryChain
* Sign up for StoryChain

### Creating storyLinks

As a user, I should be able to:

* View a random 'storyLink' and contribute a new storyLink to the chain
* Contribute to a story chain to which I have previously contributed, IF
    I have not created any of the previous 5 links in the chain.
* Reference a character within a storyLink using the @ identifier
* Reference a topic/theme within a storyLink using the # identifier
* Reference a location within a storyLink using the > identifier.
* Tag a storyLink as 'the end of a story'
* Tag a storyLink as 'nsfw'
* Tag a storyLink as '18+'

### Reading storyLinks

As a user, I should be able to:

* Access any storyLink I have previously read
* Read a 'child storyLink' of a storyLink I have previously read
* View a map that shows:
  * How the storyLinks I have read interconnect.
  * Which storyLinks have 'unread' storyLinks I can access.
  * Which storyLinks I have created.
* Upvote or downvote a storyLink
  * Toggle my vote for a storyLink between [up|down|none]
* Tag a storyLink as 'the end of a story'
* Tag a storyLink as 'nsfw'
* 'Bookmark' storyLinks for quick access
* Save a story chain by identifying beginning & end links
* Export saved story chains for access outside the app

### Social

As a user, I should be able to:

* Invite friends to add storyLinks building upon links I've created
* Add 'friends' within the app
* See storyLinks my friends have created (if I have access to the link)
* See the storyLinks my friends have bookmarked
* See which unread storyLinks point towards one of my friends' storyLinks
* Invite friends to a Saga I created.

### Sagas

As a user, I should be able to:

* Create a new 'Saga' - a full set of interconnected story chains.
  * Create the title & description for a new Saga
  * Seed a new Saga with a 'starting ring' - A set of storyLinks that create
      a looping narrative, from which every story chain in the Saga descends.
      _Using a 'starting ring' ensures that every link in a Saga has a single
      parent._
* Select which Saga to access.

### Credits

As a user, I should be able to:

* Earn 'credits' to access ancestor storyLinks by:
  * Achieving certain quality contribution goals (e.g., 1k upvotes)
  * Buy credits via micro-transaction (e.g., $1.99 per credit)
* Use 'credits' to access friends created/bookmarked storyLinks