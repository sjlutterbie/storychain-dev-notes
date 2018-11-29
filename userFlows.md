# Userflows

## Landing Page

| User action                               | Event                        |
| ----------------------------------------- | ---------------------------- |
| Click `Sign up` button                    | Load `Signup page/modal`     |
| Click `Log in` button                     | Load `Login page/modal`      |
| Click `Learn more` button *(mobile only)* | Scroll to `About Premise` |

*Add `Sign up` button at end of mobile landing page, for users who scroll?*

## Sign Up page/modal

| User action                | Event                                                        |
| -------------------------- | ------------------------------------------------------------ |
| Click `Show/hide password` | Toggles `password field` character masking                   |
| Click `Sign up` button     | Creates account, authenticates, redirects to `app interface` |

## Log In page/modal

| User action | Event |
| --- | ---|
| Click `Log In` button | Validates user; throws error or handles login |

*On 1st Log In: Directs to `User Guide`*

*On 2nd+ Log Ins: Directs to `Readindg View`*


## App Header

| User action | Event |
| --- | --- |
| Click `?` button | Load `User Guide View` |
| Click `Settings icon` | Toggle dropdown menu with `Contact` and `Logout` links |
| Click `Log out` link | Clears JWT authentication, redirects to `landing page` |
| Click `Contact` link | Opens 'mailto' link in new tab |

## Floating View Buttons

| User action | Event |
| --- | --- |
| Click `Network View` button | Load `Network View` |
| Click `Reading View` button | Load `Reading View` |

## User Guide View

| User action | Event |
| --- | --- |
| Click `Next` button | Loads next `User Guide slide` |
| CLick `Previous` button | Loads previous `User Guide slide` |
| Click `Get started` link | Loads `Reading View` |

*Biz logic will determine visibility of buttons/links*

## Reading view

| User action | Event |
| --- | --- |
| Click `Moment` component | Loads `Moment Actions` interface |

### - Moment Actions interface 

| User action | Event |
| --- | --- |
| Click `Create` button | Loads `Create Moment` form |
| Click `Switch` button | Updates `Reading View` to next longest `Story Branch` from current location |

### - Create Moment form

| User action | Event |
| --- | --- |
| Click `Cancel` button | Hides `Create Moment form` (if applicable) |
| Click `Submit` button | Adds `Moment`, reloads `Reading View` to end with newly added `Moment` |

## Network view

| User action | Event |
| --- | --- |
| Click `Moment` node | Loads `Reading View` including `Moment`, highlighting clicked `Moment`|
