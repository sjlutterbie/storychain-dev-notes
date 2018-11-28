# User Testing

## Paper Interface Test 3 (2018-11-28)

![Paper Interface Test 3](https://github.com/sjlutterbie/storychain-dev-notes/blob/master/user-feedback/paperTest3.jpg)

### Takeaways:

1. The User Guide is more concise - and much clearer. It successfully introduced
   the users to the core functions of the app, without muddying the water with
   terminology and advanced uses.
2. Highlighted a few minor UI/navigational improvements that would create a
   more streamlined experience.

### Raw notes

__Test user 1:__

* Typo: "switch branch" -> "switch branches" in User Guide 2/3.
* Should "Switch branch" direct the user to the `Network View`, from where
    they can see their current location, and choose from different branches?
  * _Good idea, but not an MVP candidate. This would be viable once more
     advanced branch sorting & optimizing is in place._
* Click on a `Moment` in `Network View` -> Switch to `Reading View`, load
  the full `Story chain` of which the moment is a part, then auto-scroll to
  highlight the moment in question.
* Include a simple visual indicator of how many alternate branches could be
  selected from any given moment?
  * _Potential MVP or MVP+1 feature._

__Test user 2:__

* Navigating between chains (knowing to go to `Network View`) may take some
    getting used to new users.
* `Create moment form` at the end of a `Story chain` shouldn't have a
  `Cancel button` (Pressing 'cancel' would simply clear & reload the form).
  * _A `Create moment form` mid-stream SHOULD have a cancel button, because
     pressing it would hide the form.`
