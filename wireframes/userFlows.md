# Userflows

## Landing Page

**Wireframe**: [./wireframes/landing.html](./wireframes/landing.html)

| User action                               | Event                        |
| ----------------------------------------- | ---------------------------- |
| Click `Sign up` button                    | Load `Signup page/modal`     |
| Click `Log in` button                     | Load `Login page/modal`      |
| Click `Learn more` button *(mobile only)* | Scroll to `About StoryChain` |

*Add `Sign up` button at end of mobile landing page, for users who scroll?*

## Signup page/modal

**Wireframe** [./wireframes/login.html](./wireframes/login.html)

| User action                | Event                                                        |
| -------------------------- | ------------------------------------------------------------ |
| Click `Show/hide password` | Toggles `password field` character masking                   |
| Click `Sign up` button     | Creates account, authenticates, redirects to `app interface` |

## App interface

**Wireframe** [./wireframes/app-interface-saga.html](./wireframes/app-interface-saga.html)

| User action | Event |
| --- | --- |
| Click `User icon` | Toggle dropdown menu with `Contact` and `Logout` links |
| Click `Log out` link | Clears JWT authentication, redirects to `landing page` |
| Click `Contact` link | Opens 'mailto' link in new tab |

### Network panel

| User action | Event |
| --- | --- |
| Click `storyLink` node | Sets `storyLink` to head of `Story Chain` list  |
| Double-click `storyLink` node | Sets `storyLink` to root of `Story Chain` list |
| Click on `unread storyLink` node | Sets `storyLink` node status to `read` |

*NOTE: Nodes, and connecting edges, associated with `storyLinks` in the
  `Story Chain` panel are highlighted in the `Network panel`.*

### Story chain panel

| User action | Event |
| --- | --- |
| Click `storyLink` component | Sets `storyLink` to head of `Story Chain` list |
| Click `Read on!` button | Selects random `unread storyLink` child of head `storyLink`, loads and sets to head of `Story Chain` list. If no `unread storyLinks` exists, selects random `read storyLink`, instead. |
| Click `Add link` button | Opens `add storyLink` modal, based on head element of `Story Chain` list |
| Click `New chain` button | Opens `add storyLink` modal, based on random unread `storyLink` |

*NOTE: All these buttons need better names!*

### 'Add storyLink' modal

**Access via display toggle at top of [./wireframes/css/app-interface.css](./wireframes/css/app-interface.css)**

| User action | Event |
| --- | --- |
| Click `Cancel` button | Closes modal window |
| Click `Submit` button | Validates entry, adds `storyLink` to DB, adds `storyLink` to head of `Story Chain` list. If new `storyLink` was based on randomly supplied `storyLink`, set supplied `storyLink` to root of `Story Chain` list | 