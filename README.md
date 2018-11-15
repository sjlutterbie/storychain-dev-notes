# StoryChain: Dev Notes

StoryChain is a collaborative storytelling platform where users can add 'storyLinks'
to story chains, follow the stories that evolve from the storyLinks they create, and
uncover how different story chains interconnect.

## User stories

* As a site visitor, I should be able to:
  * Learn about StoryChain
  * Sign up for StoryChain

* As a user, I should be able to:
  * View a random 'storyLink' and contribute a new storyLink to the chain
  * Contribute to a story chain to which I have previously contributed, IF
      I have not created any of the previous 5 links in the chain.
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
  * Tag a storyLink as '18+'
  * Reference a character within a storyLink using the @ identifier
  * Reference a topic/theme within a storyLink using the # identifier
  * Reference a location within a storyLink using the > identifier.
  * 'Bookmark' storyLinks for quick access
  * Earn 'credits' to access ancestor storyLinks by:
    * Achieving certain quality contribution goals (e.g., 1k upvotes)
    * Buy credits via micro-transaction (e.g., $1.99 per credit)
  * Invite friends to add storyLinks building upon links I've created
  * Add 'friends' within the app
  * See storyLinks my friends have created (if I have access to the link)
  * See the storyLinks my friends have bookmarked
  * Use 'credits' to access friends created/bookmarked storyLinks
  * See which unread storyLinks point towards one of my friends' storyLinks
  * Save a story chain by identifying beginning & end links
  * Export saved story chains for access outside the app
  * Submit a 'starting ring' to seed a new 'saga'
    * 'Saga' - A full set of interconnected story chains.
    * A 'starting ring' - A set of storyLinks that create a looping narrative,
        from which every story chain in the Saga descends. _Using a 'starting
        ring' ensures that every link in a Saga has a single parent._