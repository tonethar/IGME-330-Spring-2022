# Project 1 - HTML5 App of Awesomeness
## Final Deliverable

<hr><hr>

## Project 1 Links:

- [Project 1 - Checkpoint #1](p1-checkpoint-1.md)
- [Project 1 - Checkpoint #2](p1-checkpoint-2.md)
- **Project 1 - Final Deliverable**
- [Project 1 - Tips & Tricks](p1-tips.md)
- [IGME-330 - Course Code Style Requirements](330-code-style.md) 

<hr><hr>


## I. Here are the major requirements

1) Every time the user clicks the search button, this App page WILL automatically save the last term searched by the user and the third control's UI *state* in the browser's `localStorage` - this was covered in IGME-230/235 here --> [Web Apps 9 - WebStorage API](https://github.com/tonethar/IGME-230-Master/blob/master/notes/web-apps-9.md):
    - we are going to test this capability by typing in a search term, changing a value of the 3rd control, doing a search, and then closing the browser window. When we re-open the window, the user's last search term must be visible, and the rest of the UI should be in the same *state*
    - you will store this app state in an *object literal* under a single "key" named `abc1234-p1-settings` (where `abc1234` is your "banjo id")
    - storing object literals in `localStorage` is covered here - [Web Apps 9 - WebStorage API - Storing Objects with Web Storage](https://github.com/tonethar/IGME-230-Master/blob/master/notes/web-apps-9.md#iii-storing-objects-with-web-storage)
    - we also covered it in the [Week 6A `localStorage` demo](../weekly/06A.md#iv-localstorage-demo)

2) The app must have a 4th web component - and it must be `<app-navbar>` - this navbar must have "you are here" cues such as bold text

3) The app must use `fetch()` instead of `XHR`

4) The app must use either Mapbox or Firebase:
  - If you are using Mapbox, you probably should NOT do a full-screen interface like we did in the Maps II HW. Much of the time, a smaller map, and displaying more textual information, makes sense. For example, see how Yelp handles maps - https://www.yelp.com/search?find_desc=Garbage+Plate&find_loc=Rochester%2C+NY+14604
  - If you are using Firebase, you will probably be meeting that requirement with a **"Community"** page, which shows the favorites of ALL of the app's users
  - We are covering Firebase on 7B and 8A

5) The app must be easy to use, with well-labeled and obvious controls:
  - the search button is prominent, in an obvious location, stands out from the rest of the UI (give it an appropriate Bulma style for a seach button) and "looks like a button"
  - controls should have labels and/or tooltips (use the `title` attribute)

6) The app must always "let the user know what's going on" with activity indicators:
  - use the `is-loading` Bulma class to get a "spinner" on a button - https://bulma.io/documentation/elements/button/
  - use a Bulma "Indeterminate Progress Bar" - https://bulma.io/documentation/elements/progress/#indeterminate
  - if a search result on a card is *favorited*, then the "Favorite Me!" button should change state to indicate that particular result can not be favorited again

7) The app must "fail gracefully" and errors must be communicated to the user - for example:
  - "No results found" message if a search comes back with no results
  - "Please enter a search term" if the user clicks the search button without typing anything in

8) The app must have "Impact":
  - it serves a purpose - i.e it should be useful to someone
  - it is easy to use, functional, and aesthetically pleasing
  - it should be (or approaching) "portfolio quality" - something you would be able to show a potential employer

<hr>

## II. Code Standards
- All project files MUST adhere to this --> [IGME-330 - Course Code Style Requirements](330-code-style.md) 
- All `<script>` tags MUST be in the `<head>` section of the document and be of `type="module"`
- All web components are in their own JS file. Component file names MUST match their tag name - example - the file that contains the `<sw-card>` code must be named **sw-card.js**
- All web components must accept at least 1 *parameter* and utilize it. A parameter can be passed in via slots, attributes or via an object property
- Simplify the code in your web components and eleminate any redudant code:
  - for example, if you are just using slots and there's no JavaScript in the component, you probably don't need any of the lifecycle methods, nor do you even need a `render ()` helper method. The `template` and a `constructor()` should suffice
- All HTML pages must pass HTML validation - this includes your web components too
  - be sure to test your **app.html** page AFTER you've loaded in some results and instantiated - for example - some `<sw-card>` component instances 
  - https://validator.w3.org/
- All CSS must pass CSS validation
  - https://jigsaw.w3.org/css-validator/

<hr>

## III, Rubric (coming soon!)

- "Impact" is weighed heavily 
- All requirements from previous checkpoints are still in effect, and you will lose points for not meeting them
