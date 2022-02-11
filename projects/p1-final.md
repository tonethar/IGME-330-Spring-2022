# Project 1 - HTML5 App of Awesomeness (DRAFT)
## Final Deliverable

<hr>

## I. Here ae the major requirements
- The app must have a 4th web component - `<app-navbar>`
- The app must use `fetch()` instead of `XHR`
- The app must use either Mapbox or Firebase
- The app must be easy to use, with well-labeled and obvious controls:
  - the search button is prominent, in an obvious location, stands out from the rest of the UI (give it an appropriate Bulma style for a seach button) and "looks like a button"
  - controls can have labels and/or tooltips (use the `title` attribute)
- The app must always "let the user know what's going on" with activity indicators
  - use the `is-loading` Bulma class to get a "spinner" on a button - https://bulma.io/documentation/elements/button/
  - use a Bulma "Indeterminate Progress Bar" - https://bulma.io/documentation/elements/progress/#indeterminate
- The app must "fail gracefully" and errors must be communicated to the user - for example:
  - "No results found" message if a search comes back with no results
  - "Please enter a search term" if the user clicks the search button without typing anything in
- The app must have "Impact":
  - it serves a purpose - i.e it should be useful to someone
  - it is easy to use, functional, and aesthetically pleasing
  - it should be (or approaching) "portfolio quality" - something you would be able to show a potential employer
