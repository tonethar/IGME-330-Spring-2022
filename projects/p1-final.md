# Project 1 - HTML5 App of Awesomeness (DRAFT)
## Final Deliverable

<hr>

## I. Here are the major requirements
- The app must have a 4th web component - `<app-navbar>`
- The app must use `fetch()` instead of `XHR`
- The app must use either Mapbox or Firebase:
  - If you are using Mapbox, you probably should NOT do a full-screen interface like we did in the Maps II HW. Much of the time, a smaller map, and displaying more textual information, makes sense. For example, see how Yelp handles maps - https://www.yelp.com/search?find_desc=Garbage+Plate&find_loc=Rochester%2C+NY+14604
  - If you are using Firebase, you will probably be meeting that requirement with a **"Community"** page, which shows the favorites of ALL of the app's users
- The app must be easy to use, with well-labeled and obvious controls:
  - the search button is prominent, in an obvious location, stands out from the rest of the UI (give it an appropriate Bulma style for a seach button) and "looks like a button"
  - controls can have labels and/or tooltips (use the `title` attribute)
- The app must always "let the user know what's going on" with activity indicators:
  - use the `is-loading` Bulma class to get a "spinner" on a button - https://bulma.io/documentation/elements/button/
  - use a Bulma "Indeterminate Progress Bar" - https://bulma.io/documentation/elements/progress/#indeterminate
- The app must "fail gracefully" and errors must be communicated to the user - for example:
  - "No results found" message if a search comes back with no results
  - "Please enter a search term" if the user clicks the search button without typing anything in
- The app must have "Impact":
  - it serves a purpose - i.e it should be useful to someone
  - it is easy to use, functional, and aesthetically pleasing
  - it should be (or approaching) "portfolio quality" - something you would be able to show a potential employer

<hr>

## II. Code Standards
- All project files MUST adhere to this --> [IGME-330 - Course Code Style Requirements](330-code-style.md) 
- All `<script>` tags MUST be in the `<head>` section of the document and be of `type="module"`
- All web components are in their own JS file. Component file names MUST match their tag name - example - the file that contains the `<sw-card>` code must be named **sw-card.js**
- All HTML pages must pass HTML validation - this includes your web components too
  - be sure to test your **app.html** page AFTER you've loaded in some results and instantiated - for example - some `<sw-card>` component instances 
  - https://validator.w3.org/
- All CSS must pass CSS validation
  - https://jigsaw.w3.org/css-validator/
