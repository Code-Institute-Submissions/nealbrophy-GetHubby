# GetHubby
Code Institute User Centric Frontend Develtopment: Milestone Project One

This is an imagined dating site for developers and specificially geared towards users of GitHub leveraging the existing social & community aspects of same. The goal is to have a site which appeals to developers by using industry lingo and to allow users to sign-up via existing, commonly used industry tools (i.e. GitHub).

## Demo
Click [here](https://nealbrophy.github.io/GetHubby/) to go to the live demo.

<img src="https://github.com/nealbrophy/GetHubby/blob/master/images/ipad.gif" alt="site demo on ipad" width="300px" align="left">

<img src="https://github.com/nealbrophy/GetHubby/blob/master/images/iphone.gif" alt="site demo on iphone" width="200px" align="center">


--- 
## UX
 
The site is intended to be simple and minimalistic while also colourful and fun. The information should be short and to the point but with a light-hearted tone where appropriate. Text should use industry terminology to present an industry-specific focus.

### User Stories:
- As a single person, I want a modern and appealing site which is simple to navigate.
- As a developer, I want a site that caters to my interests and is clearly aimed at people like me.
- As a modern user, I want a mobile-friendly site that looks as good on small screens as large.

### Strategy

The goal of the site was to create a dating site which might appeal to developers and also to lay the groundwork for a project-site that could be used again as I tackle more advanced subjects.

### Wireframes

The initial wireframe was intended to outline the basic structure of the site and took inspiration from several popular current dating sites such as [EliteSingles](https://dating.elitesingles.com/), [Match.com](https://ie.match.com/), and [OKCupid](https://www.okcupid.com/). The second wireframe took the structure from the first, simplified it somewhat, and added some style/colour.

<img src="https://github.com/nealbrophy/GetHubby/blob/master/wireframes/wireframe-1-bw.png" alt="wireframe-1" width="318px" align="left">

<img src="https://github.com/nealbrophy/GetHubby/blob/master/wireframes/wireframe-2-colour.png" alt="wireframe-2" width="400px" align="center">


---

## Features

The navbar is responsive and will switch to a hamburger menu on small screens. 

The hero section contains an eye-catching jumbotron slideshow with images of a variety of possible users of site. A mock-typing animation was added to the text overlayed on the slideshow to suggest a relation to coding (and more specifically GitHub commands).

On med & large screens the about section contains simple, colourful flip-cards with a short title (and icons representing the theme of the title) on the front and a short summary of the feature in question on the back. One small screens the flip cards are replaced by a collapsing list.

The testimonials section shows a circular image of imagined couples beside a short quote from each couple. The button beneath each quote opens a mock Q&A with the couple (bootstrap-modal on larger screens, bootstrap-collapse on smaller screens).

The contribute section links to this GitHub repo. The sign-up section is made to look like a code-editor window with mock-HTML text.

---
 
### Existing Features

- Carousel with typing animation overlaid
- Links to relavant sections with smooth scroll
- Flip-cards
- Modal/Collapse for couple Q&As depending on screen size
- Buttons display a popout icon relating to the content/target of said button.
- On large screens there is an arrow icon with hover.css effect to highlight that additional content is below and links to the next section.

### Features Left to Implement

Once I've progressed in the JavaScript module and further I would like to add some more advanced features such as:
- A separate, customized modal for the Member Login.
- Randomised elements such as the color pallete for the flip-cards and the testimonials (couple images/names/quotes).
- GitHub OAuth integration, or at least the appearance of such. 
- A database of mock profiles and the ability to actually run through a sign-up process.

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

The site has been developed using the mobile first approach with responsive elements where possible and media queries when necessary. All changes to the site were tested in Google Chrome, Firefox, Opera, Vivaldi, and Samsung Internet browsers (leveraging the developer tools in each) and across Windows (desktop), Linux (desktop & laptop), and Android operating systems (mobile).

When testing the breakpoints for the Testimonials section I discovered that if one of the Collapse Q&As (xs & s screens) was expanded *before* the page width was increased to the point that the Modal Q&As (md+) were supposed to take over, the expanded Collapse would remain visible. This was due to my having added the bootstrap "d-md-none" class to the Collapse buttons but not the collapse body itself. It was resolved by populating that class where necessary.

During testing I found that some absolutely positioned elements had moved up/down further depending on which browser was used. The most consistant explanation I found for this was that absolutely positioned elements need to have a relatively positioned parent element. Making this change mitigated but did not eliminate the browser variance. Small variances in position at different screen sizes was addressed using media queries. Icon position was tested using the "emulated devices" available in Chrome and Firefox dev tools as well by manually resizing using the "responsive" setting.

The button hover effect was initially implimented using "position" only but (similar to the icon issue mentioned above) I found that the positioning wasn't consistent across all browsers. The most reliable method  of resolving the issue that I found was to use a combination of positioning and CSS Grid. This was tested using an the above mentioned browsers & devices to insure that hover effect was consistent.

The Email field in sign-up form correctly prompts for valid email address format. Password field correctly hides typed text.

The faux-code-editor in the sign-up section includes line numbers on the right-hand side on larger screens to clearly illustrate what the window is supposed to be. However, these numbers would cause the overall structure of the window to break on smaller screens so the numbers are hidden in those cases. This was tested using the responsive sizing in Chrome/Firefox dev tools and by looking up the GitHub pages on an Samsung Galaxy S10 device.

HTML & CSS were validated using the W3C online tools [here](https://validator.w3.org/nu/) and [here](https://jigsaw.w3.org/css-validator/) respectively.

### Remaining bugs

There's a small flicker on the left hand side of the bootstrap carousel when changing slides which I have been unable to fix.

## Deployment

GetHubby is hosted on GitHub pages and is deployed from the master branch. Any changes committed to the master branch will automatically update on the GitHub deployment.

To run the site locally you can clone it using the following instructions:
- Create a folder in the desired location on your computer.
- Open a terminal ([Mac instructions](https://macpaw.com/how-to/use-terminal-on-mac)|[Windows instructions](https://www.quora.com/How-do-I-open-terminal-in-windows)|[Linux instructions](https://www.howtogeek.com/howto/22283/four-ways-to-get-instant-access-to-a-terminal-in-linux/))
- Navigate to the folder you created using `cd` command (e.g. `cd ~/Documents/GetHubby`)
- Type `git init`
- Next type `git clone https://github.com/nealbrophy/GetHubby`
- To break the link between your local copy and the repo at https://github.com/nealbrophy/GetHubby type `git remote rm origin`


## Credits

### Content
All text content was created by me. The modified Octocat images in the Testimonial and Contribute section were created by me for the purposes of this educational site only.

### Media
- [Pexels](https://www.pexels.com/)
    - testimonials-couple-1 Photo by Vasyl Potochnyi from Pexels
    - testimonials-couple-2 Photo by Gustavo Peres from Pexels
    - testimonials-couple-3 Photo by Gustavo Peres from Pexels
    - carousel-3-lg Photo by Brett Sayles from Pexels
    - carousel-2-sm Photo by Luis Fernandes from Pexels
    - carousel-2-lg Photo by juan mendez from Pexels
    - carousel-1-lg Photo by fauxels from Pexels
    - carousel-1-sm Photo by Innoh Khumbuza from Pexels
    - carousel-3-sm Photo by Daria Shevtsova from Pexels
- [Pixabay](https://pixabay.com/)
    - about-section-bg Image by Pexels from Pixabay


### Acknowledgements
- Typewriter effect inspired by [this CSS-Tricks article](https://css-tricks.com/snippets/css/typewriter-effect/) with simplified implementation taken from [this instructional video by Codingflag](https://www.youtube.com/watch?v=6vOJoAmbza0).
- Flip cards from [this W3C tutorial](https://www.w3schools.com/howto/howto_css_flip_card.asp)
- GITHUB®, the GITHUB® logo design, OCTOCAT® and the OCTOCAT® logo design are exclusive trademarks registered in the United States by GitHub, Inc.

## This student project and any original content therein is for educational use only ##
