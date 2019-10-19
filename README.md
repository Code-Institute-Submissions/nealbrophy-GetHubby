# GetHubby
Code Institute User Centric Frontend Develtopment Milestone Project One

This is an imagined dating site for developers and specificially geared towards users of GitHub leveraging the existing social & community aspects of same. The goal is to have a site which appeals to developers by using industry lingo and to allow users to sign-up via existing, commonly used, industry tools (e.g. GitHub, StackOverflow etc)

[Go to GetHubby](https://nealbrophy.github.io/GetHubby/)

 
## UX
 
The site is intended to be simple and minimalistic while also colourful and fun. The information should be short and to the point but with a light-hearted tone where appropriate. Text should use industry terminology to present an industry-specific focus.

User Stories:
- As a single person, I want a simple and easy to navigate site.
- As a developer, I want it to be clear that the site/service is aimed at people like me.


++++This section is also where you would share links to any wireframes, mockups, diagrams etc. that you created as part of the design process. These files should themselves either be included in the project itself (in an separate directory), or just hosted elsewhere online and can be in any format that is viewable inside the browser.+++

## Features

The navbar is responsive and will switch to a hamburger menu on small screens. 

The hero section contains an eye-catching jumbotron slideshow with images of a variety of possible users of site. A mock-typing animation was added to the text overlayed on the slideshow to suggest a relation to coding (and more specifically GitHub commands).

The about section contains simple, colourful flip-cards with a short title (and icons representing the theme of the title) on the front and a short summary of the feature in question on the back.

The testimonials section contains shows a circular image of imagined couples beside a short quote from each couple. The button beneath each quote opens a mock Q&A with the couple (bootstrap-modal on larger screens, bootstrap-collapse on smaller screens).

The sign-up section is made to look like a code-editor window with mock-HTML text.
 
### Existing Features
- Carousel with typing animation overlaid
- Links to relavant sections with smooth scroll
- Flip-cards
- Modal/Collapse for couple Q&As depending on screen size

+++For some/all of your features, you may choose to reference the specific project files that implement them, although this is entirely optional.

+++In addition, you may also use this section to discuss plans for additional features to be implemented in the future:

### Features Left to Implement


## Technologies Used

- [Bootstrap](https://getbootstrap.com/)
    - The project uses **Bootstrap** framework to simplify the initial layout and include advanced features such as the jumbotron and carousel.
- [Hover.css](http://ianlunn.github.io/Hover/)
    - The project uses the **Hover.css** collection to add appealing animations to icons & buttons.
- [Font Awesome](https://fontawesome.com)
    - The project uses **Font Awesome** for attractive and simple icons.
- [Google Fonts](https://fonts.google.com/)
    - The project uses **Google Fonts** for custom typefaces.

## Testing

+++In this section, you need to convince the assessor that you have conducted enough testing to legitimately believe that the site works well. Essentially, in this part you will want to go over all of your user stories from the UX section and ensure that they all work as intended, with the project providing an easy and straightforward way for the users to achieve their goals.

+++Whenever it is feasible, prefer to automate your tests, and if you've done so, provide a brief explanation of your approach, link to the test file(s) and explain how to run them.

+++For any scenarios that have not been automated, test the user stories manually and provide as much detail as is relevant. A particularly useful form for describing your testing process is via scenarios, such as:

+++1. Contact form:
    1. Go to the "Contact Us" page
    2. Try to submit the empty form and verify that an error message about the required fields appears
    3. Try to submit the form with an invalid email address and verify that a relevant error message appears
    4. Try to submit the form with all inputs valid and verify that a success message appears.

+++In addition, you should mention in this section how your project looks and works on different browsers and screen sizes.

+++You should also mention in this section any interesting bugs or problems you discovered during your testing, even if you haven't addressed them yet.

+++If this section grows too long, you may want to split it off into a separate file and link to it from here.

## Deployment

+++This section should describe the process you went through to deploy the project to a hosting platform (e.g. GitHub Pages or Heroku).

+++In particular, you should provide all details of the differences between the deployed version and the development version, if any, including:
- Different values for environment variables (Heroku Config Vars)?
- Different configuration files?
- Separate git branch?

+++In addition, if it is not obvious, you should also describe how to run your code locally.


## Credits

### Content


### Media
- [Pexels](https://www.pexels.com/)
    - adults-bald-bouquet Photo by Vasyl Potochnyi from Pexels
    - affection-beach-couple Photo by Gustavo Peres from Pexels
    - couple-facial-hair-garden-2440069 Photo by Gustavo Peres from Pexels
- [Pixabay](https://pixabay.com/)
    - black-and-white-2590810_1920 Image by StockSnap from Pixabay
    - couple-1210023_1920 Image by Free-Photos from Pixabay
    - code-1839406_1920 Image by Pexels from Pixabay
- [Unsplash](https://unsplash.com/)
    - diego-rezende-CFIv79QxPjA-unsplash Photo by Diego Rezende on Unsplash

### Acknowledgements
- Typewriter effect inspired by [this CSS-Tricks article](https://css-tricks.com/snippets/css/typewriter-effect/) with simplified implementation taken from [this instructional video by Codingflag](https://www.youtube.com/watch?v=6vOJoAmbza0).
- Flip cards from [this W3C tutorial](https://www.w3schools.com/howto/howto_css_flip_card.asp)
+++- I received inspiration for this project from X
