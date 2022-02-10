# Project 1 - VanillaJS App of Awesomeness - DRAFT!
## Checkpoint #2 - Working Prototype - DRAFT!

***\*THIS DOCUMENT IS A DRAFT! - IT IS NOT FINAL\****


## I. Rubric First
- Worth 5% of Final Grade
- Out of 20 points

    A. (0-2) 4 pages (Home, App, Favorites, Documentation) with required content (0-2)

    B. (0-2) Bulma is utilized for navigation, text, and buttons (0-2)

    C. (0-2) Mobile Friendly navigation with functioning hamburger menu (**hamburger.js**) on all pages

    D. (0-2) Home & Documentation pages have required content

    E. (0-2) App page functions and has a search button and a text field, and at least one other filtering control

    F. (0-2) App page results are displayed in a "card" component 

    G. (0-2) App utilizes 3 components (including the card component above)

    H. (0-2) App page UI state is preserved in `localStorage` inside a single object literal. The `localStorage` key (there is only one) is unique

    I. (0-2) Code files/standards: ES 6 Modules, at least 3 web components, fetch(), follows code standards, files: app.js, hamburger.js, utils.js (contains Ajax and any other factored out code), 3 **XYZ-component.js** files

    J. (0-2) Follows 330 [Code Standards](./code-style.md)

<hr>


## II. Content Requirements - *Home page*

- Tell the user what your app does
- Have some sort of "brand" for your page:
  - it could be a `navbar-brand` like in the Bulma template - an image or font awesome icon
  - it could be a stylized logo you create yourself
- You might want to use a Bulma `hero`
- There must be at least one image on this page (in addition to whatever appears in `navbar-brand`)
- *Optional: Consider adding some sort interactive content or "flare" to this page - an image carousel, random quotes from happy users, etc*

<hr>

## III. Functional Requirements - *App page*

1. You must use at least **ONE** web service API in your completed project:

2. On the app page, you WILL automatically save the last term searched by the user and other UI *state* in the browser's local storage - this was covered in IGME-230/235 here --> [Web Apps 9 - WebStorage API](https://github.com/tonethar/IGME-230-Master/blob/master/notes/web-apps-9.md):
    - this will also be true of the other controls on the page (&lt;select> tags, radio buttons, checkboxes etc)
    - we are going to test this capability by typing in a search term, selecting some checkboxes, doing a search, and then closing the browser window. When we re-open the window, the user's last search term must be visible, and the rest of the UI should be in the same *state*

3. Other required controls - there WILL be a MINIMUM of 3 controls that a user can use to filter and display the results. Search buttons or similar don't count towards the 3 controls. For example, [GIF Finder](https://github.com/tonethar/IGME-230-Master/blob/master/notes/HW-gif-finder.md) has these controls:
    - a search button (which doesn't count)
    - a search term field (&lt;input>) that the user types into
    - a pulldown (&lt;select>) that the user can use to limit the number of results

    -  **So you will need at least one additional kind of control. What kind of control to use depends on what parameters the web services will allow you to search them on. Here are some ideas:**
       - a **rating** pulldown - if we had this on the GIPHY HW then a user would be able to choose between viewing "G" and "PG" videos for example
       - a **sort by** pulldown to allow the user to view the results sorted A->Z, Z->A, by date, etc 
       - a **date** chooser to filter the results by date - https://developer.mozilla.org/en-US/docs/Web/HTML/Element/input/date
       - **next** and **previous** buttons - another really nice option is to allow the user to "page" through large numbers of results. In the GIPHY HW did you notice that we always get the same 100 "cat" GIFs back when we search?
         - This is because there are ***thousands*** of cat GIFs on GIPHY, and if we don't otherwise specify we will always get them returned from the web service starting at index 0, which means we always get the first 100 (index 0-99) back.
         - We can instead write code that requests a higher starting index.
         - In the GIPHY API this can be done by tracking and adding an `offset` value to the query string that is sent over to the API.

<hr>


## IV. Functional Requirements - *Favorites page*

- The favorites (or lists or bookmarks) WILL be stored in `localStorage` and can be viewed on this page
- There MUST be a be a *Delete* button that clears `localStorage` (thus removing the favorites from the page)
- The user will probably be able to interact with the favorites in some other way - "View Next 5" and "View Previous 5" buttons etc... especially if there are a lot of favorites.
- *Optional - the user can also sort, re-order and delete individual favorites*

<hr>

## V. Content Requirements - *About/Documentation page* 
- Keep your project proposal from checkpoint #1 - and put it under a PROPOSAL subheading
- Have the following additional 6 sub-headings on your page (see the [example Desktop screenshots of sources.html](#desktop-sources-screenshots) below
  - PROJECT REQUIREMENTS:
    - provide a link to this page
  - RESOURCES UTILIZED:
    - cite any and all resources you used on this project, the specific link, including:
      - fonts and images
      - reference sites - ex. developer.mozilla.org
      - "help" sites - ex. stackoverflow.com
      - code snippet sites - ex. CodePen or gists.github.com or copying starter code from the Bulma site etc
      - tutorial sites - ex. w3schools.com
      - video sites - ex. YouTube or LinkedIn Learning or Udemy
      - blog postings etc
    - Exception: you need not cite any IGME-330 resources/tutorials/HWs:
      - but you MUST cite resources from other courses including IGME-235 
  - API:
    - Link to the API Home, documentation, and endpoints used (but don't include your API key!)
  - NOTEWORTHY: (you can leave this section blank for now)
    - Talk the project up - list the technologies you used (web components, Bulma, fetch, promises, etc)
    - Be sure to emphasize what you did outside of what we covered in class
  - GRADING: (you can leave this blank for now)
    - Describe how you met project requirements
    - Describe how you went "above and beyond" project requirements
    - In the comments field of the dropbox, grade your Project 1 submission
  - TO DO:  (you can leave this blank for now)
    - List any features that you would have liked to add if you had time
    - These could potentially be added to the app for Project 2, or over break/summer when you have time

<hr>

## VI. Sample Screenshots

<a id="desktop-screenshots"/>

### VI-A. Desktop Version

<hr>

**about.html**

![screenshot](https://github.com/tonethar/IGME-330-Fall-2021/blob/main/projects/_images/p1-desktop-ss-1.png)

<hr>

**app.html**

![screenshot](https://github.com/tonethar/IGME-330-Fall-2021/blob/main/projects/_images/p1-desktop-ss-2.png)

<hr>

**favorites.html**

![screenshot](https://github.com/tonethar/IGME-330-Fall-2021/blob/main/projects/_images/p1-desktop-ss-3.png)

<hr id="desktop-sources-screenshots">

**sources.html**

![screenshot](https://github.com/tonethar/IGME-330-Fall-2021/blob/main/projects/_images/p1-desktop-ss-4.png)

![screenshot](https://github.com/tonethar/IGME-330-Fall-2021/blob/main/projects/_images/p1-desktop-ss-4B.png)

![screenshot](https://github.com/tonethar/IGME-330-Fall-2021/blob/main/projects/_images/p1-desktop-ss-4C.png)

<hr>

### VI-B. Mobile Version

<hr>

**about.html**

![screenshot](https://github.com/tonethar/IGME-330-Fall-2021/blob/main/projects/_images/p1-mobile-ss-1.png)

<hr>

**app.html**

![screenshot](https://github.com/tonethar/IGME-330-Fall-2021/blob/main/projects/_images/p1-mobile-ss-2.png)

<hr>

**favorites.html**

![screenshot](https://github.com/tonethar/IGME-330-Fall-2021/blob/main/projects/_images/p1-mobile-ss-3.png)

<hr>

**sources.html**

![screenshot](https://github.com/tonethar/IGME-330-Fall-2021/blob/main/projects/_images/p1-mobile-ss-4.png)


<hr>


<!--
## II. Project 1 Final 
- Worth 15% of Final Grade 

    A. The Favorites Page now functions - it will use localStorage to storage user specific app favorites locally. All of the app favorites are preserved in localStorage inside of the single object literal used in Project 1 Checkpoint. The favorites will be displayed using a custom web component

    B) The App will utilize Firebase to create a Community page

    **OR**

- The App will utilize Mapbox and display location data that is returned by a web service. The app will not solely display hard-coded (or locally stored) location data

    C) App navigation now has "You are here cues" (ex. **bold** text or a different colored background, NOT literally the words "You Are Here")
    
    D) App navigation is now a web component

    E) App Page Improvements:

    1. animated button or element letting the user know when a search is going on

    F) Design & Interaction 

    1. Pleasing graphic design
    1. Users must be able to figure out how to use the app with minimal instruction
      - be sure to provide instruction and tooltips if necessary
    1. User errors must be handled gracefully
      - for example, if the user forgets to type in a search term before clicking the Search button, the app should tell the user something like "Please enter a search term first"
    1. Users must know what *state* the app is in at all times

<hr>

-->

## ***Fall 2021 Reference***

- https://github.com/tonethar/IGME-330-Fall-2021/blob/main/projects/project-1.md
- https://github.com/tonethar/IGME-330-Fall-2021/blob/main/projects/project-2.md
- https://github.com/tonethar/IGME-330-Fall-2021/blob/main/projects/p1-tips.md
