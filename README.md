# ODX Trello theme
Allowing Trello boards to be (preset) theme-able and adding additional functionality to them.

## Requirements and usage
### Installation
Currently ODX-TT is not a stand alone plugin or such, it requires browser plugins. 

The plugins I currently use and reccomend are the following:

 - Stylish - for implementing CSS changes required
 - Tampermonkey - for running the javascript required.
 
At present testing is done only on the afore mentioned plugins in the latest version of Chrome under windows 8.

### Instructions/functionality 

Some of the header bar is slightly re-arranged. 

The new features are available to the right of the search box the four buttons are as follows:

Any active button/selection will be  highlighted with a white border

- Single-user mode denoted by a "|" in a box. 
    - This mode takes the current active user (as logged in) and partially hides any cards that are not marked with your account active on them.
- Multi-user mode denoted by a "|||" in a box.
    - This button toggles Single-user mode off and expands all cards to normal size.
- Style sheet selection is an empty box at present.
    - Clicking this button will toggle the stylesheet selection buttons - an assortment of coloured buttons
    - The stylesheet buttons are coloured in line with the image they set the background to
- Further config settings can be accessed via the cog buttong
    - *this button is currently not active - temporarily*

### Licensing 

Not currently available - until further notice: use and distribute as you see fit - have at it in any way shape or form.

## Current version: ODX-TT v0.0.4

*Please note: current version temporarily unavailable as I make the changes required for this to be hosted on github - ie no proprietry/copyrighted imagery or such - some was used during my personal only usage/testing. Also a couple of cookie issues I want resolved before outputting this too *

### New in this version
- new base template style changes
- style selector management minify - minimise/group all sub styles when not selecting style
- new config panel - only colour is functional at this stage - colours set globally via cookies (not completely implemented yet)
- add functionality to select whether viewing board by default view (group) or new view single user (hides tasks not associated with user viewing board in either slimline mode or complete removal)

### Features
- exposes card numbers in the main board UI so you are able to reference card numbers in other software/conversations/etc.
- allow users to switch between single user and all user/group views
  - single user mode minifies all other cards not assigned to user - highlights only user cards - most card functionality still available
  - designed to unclutter busy card boards so you can get at your items easily and efficiently - hopefully :)
  - all user / group  user view is default trello card view
  - currently set on an entire site level 
  - state saved via cookie 
- colour/style selection - 
  - currently set on an entire site level 
  - state saved via cookie
- style changes to interface - for better or worse ;)

### to do list - /.plan
- release via github/open source
- images for sub-themes
    - icon images (cog)
    - host images - stop hot linking (this is only being done during minimized testing - naughty as it is)
    - create new core style backgrounds - ie no licensing/ownership issues
- base theme style colour removal
- style overrides for sub-themes - colours back in
- enable style per board selection - ie have a different style applied to any board - not globally
    - investigate local storage vs cookies - don't want ODX cookies to potentially overwrite trello cookies or conflict with other trello plugins
    - eventually investigate alternative also - to allow users to keep their theme regardless of where they are - optional! - not forced
- add functionality to allow user to set a "team" for team based boards - some boards have dummy users setup as team catch alls - such as an all of organisation tactical board. Letting the user set an account as a team will allow for the user to filter a board to only see cards assigned to his/her team.

###long term roadmap - blue sky
- possibly bundle into chrome plugin
- user account (or code) / allow you to take settings with you wherever you go
- custom user themes - import your own CSS
