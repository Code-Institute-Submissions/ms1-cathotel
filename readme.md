# MS1: The Cat Hotel.

User Centric Frontend Web Development Project Submission

## Access

View the project live: [here](http://rbsam176.github.io/ms1-cathotel/)

View the Github repo: [here](https://github.com/rbsam176/ms1-cathotel)

## Table of Contents
* [UX](#ux)
    * [Strategy](#Strategy)
        * [Business Objectives](#Business-Objectives)
        * [User Stories](#User-Stories)
    * [Scope](#scope)
        * [Current Features](#current-features)
        * [Long-term Vision](#long-term-vision)
    * [Structure](#structure)
    * [Surface](#surface)
        * [Animation](#animation)
        * [Colour](#colour)
        * [Typography/Icons](#typographyicons)
* [Accessibility](#accessibility)
* [Technologies Used](#technologies-used)
* [Resources](#resources)
* [Testing](#testing)
    * [Validation](#validation)
    * [Bugs](#bugs)
    * [Cross-browser Compatability](#cross-browser-compatability)
    * [Lighthouse](#lighthouse)
    * [Accessibility](#accessibility)
* [Deployment](#deployment)
* [Final Product](#final-product)
* [Credits & Attributes](#credits--attributes)

## UX

### Strategy

#### Business Objectives
<details>  
<summary>To increase the number of bookings</summary>
Prior to website creation, the primary method of booking was by phoning the number listed on social media.
</details><br>


<details>
 <summary>To provide key information all in one location</summary>
 Until now, all information regarding location, phone number etc. was kept on directory websites like Tripadvisor/Yelp.
</details><br>


<details>
 <summary>To be able to control the branding of the business</summary>
 The business can select which photos are to be seen by potential customers as opposed to user-submitted photos on social media.
</details><br>

#### User Stories
The project is for a fictional cattery business based in South West England. The website serves multiple purposes:
* Attract new customers by discovering the website via Google searches, review websites or social media.
* Facilitate customers making a booking request for a stay for their cat.
* Provide some background information on both the owners and the cattery.
* Exhibit multiple photos that convey what the cattery is like before a customer decide to book.
* Allow customers to contact the business for additional questions before they decide to book.

### Scope

#### Current Features
* Immersive photographic experience, allowing the photos to be a primary source of colour to the overall site design.
  * Every photo is high resolution.
  * Every photo is linked so the viewer can see it full-size.
* Booking form located at the top so it is immediately available upon arival.
  * Booking form location and structure changes depending on the breakpoint for a better mobile experience.
* Navigation designed for both desktop and mobile experiences.
  * When in mobile view, the navbar is fixed at the top for easy access.
  * When in mobile view, a 'book' nav item appears for easy booking.
  * Smooth-scrolling enabled (browser-compatability limited)
  * Responsive 2 column grid detailing pricing and terms that stacks vertically when resized to a smaller screen size.
* Responsive grid of publications the cattery has been featured in to provide a sense of legitmacy and popularity to the business.
* Selected testimonial with link to source for customer verification
* Compact about section with accompanying photographs showcasing the incredible surrounding garden.
  * Photos in about section turn into a carousel for a better mobile experience.
* Responsive grid of products that business is partnered with to provide potential customers the knowledge of what products are used while the cat is in care.
  * This also helps the customer understand the quality of the experience, that good well-known food brands are used.
* Gallery showcasing photos of both the exterior and environment of the cattery, but also some of the cats that have previously stayed.
  * Gallery turns into a carousel in mobile view for a better mobile experience.
* Dedicated contact section that provides the customer with a map of the location, a contact form for questions and opening hours.
  * This section of 3 column changes to a vertical stack when in mobile view to allow enough space for each sub-section.
* Footer contains up arrow to easily get back to the top of the site, especially useful on mobile as it saves the user continuinally scrolling up.
* Footer contains social media links for customers to subscribe or see user-generated content.
  * The footer structure changes to be stacked vertically at different breakpoints.


#### Long-term Vision
* Dynamic testimonials. This could be done either by changing on each visit/time of day, using a carousel that continually scrolls through, or embedding an external review source such as Tripadvisor/Yelp.
* Having a dark-mode version of the site that automatically detects what mode the device is in.
* Including an AR experience - there are an increasing amount of web-based AR technologies available, which would offer a great immersive insight for the customer.
* Customer account system, this could allow:
  * Loyalty discounting by keeping track of bookings
  * See photos of your cat during its stay
  * See log of previous bookings, retrieve invoices 
* Booking calendar so the customer can see live availability without the need to 'request' a booking, they would receive an immediate confirmation
* Payment system so they can pay a deposit through the website as opposed to in-person on the premises
* Review system so the testimonials section can run independent of third party websites such as TripAdvisor/Yelp
* Improve Performance of load times, using Google Lighthouse as a metric to track any improvements. A few ways to approach this would be:
  * To use Javascript to dynamically change the resolution of images to be appropriate for the screen size viewing them. 
  * To convert the images to a next-gen image format such as WebP, which is steadily gaining more browser support (Safari 14 just announced support). Until WebP gains complete cross-browser support, writing in a fallback image format would be ideal to avoid some users not being able to load any images.

## Structure
 
I made the decision to have the site appear all on one page with clear sections for easy navigation.  
This decision was partly influenced by design, as I felt having the section sit next to each other with photographs surrounding them was visually more appealing, but also because I felt it made for a better mobile experience as everything can be loaded in one instance and the user can access different sections without waiting.  
The order of the sections was intentional, I wanted the ability to book to be the first container visible upon arrival so the user didn't have to spend time searching in order to book.  
Rather than immediately going to About/Gallery/Contact, I wanted to include sub-sections that appear when the user is transitioning from one section to another. This took the form of a grid showcasing the publications that the business has been featured in, and a grid of products the cattery uses during its operation. Having this works very well with a one-page design as opposed to multiple pages as this content isn't worthy of a page of it's own, and will be more frequently seen when it appears between sections of importance.

## Skeleton

### Wireframing
I started the project by first creating a wireframe with Balsamiq, this helped me visualise how the structure of the page would look on all device sizes.  

You can see how the final design retains a lot of the structure from the wireframe, but also how it has deviated in the way it responds at different breakpoints. This was as a result of learning and becoming more comfortable with Bootstrap and allowing it to influence the best structure based on its own grid system.

*Click the image to see it full-size.*  

<img src="assets/images/cattery-all-media-types.png" alt="submit button" width="472" height="732" />

## Surface

### Animation

* Smooth scrolling enabled so the transition from clicking a link to the page arriving at the anchor isn't abrupt. This is unfortunately not compatible with Safari unless Javascript is applied.

<img src="assets/images/smoothscroll.gif" alt="GIF of smooth scrolling"/>

* Applied an opacity filter to all links with a smooth fade (0.3s) to avoid an abrupt changing of hue.

<img src="assets/images/hoverfade.gif" alt="hover effect"/>

### Colour

There is a light accent colour of a gradiented-blue throughout the site found on the submit buttons, but primarily I wanted the colour to derive from the photos used extensively throughout rather than from text or icons.

#### Buttons
##### Default:  
#0B44EF <img src="assets/images/swatch-0B44EF.jpg" alt="swatch of #0B44EF"/>  
#007dfa <img src="assets/images/swatch-007dfa.jpg" alt="swatch of #007dfa"/>   
*(-45 degree angle)*  
##### Hover:  
`opacity: 0.9;`  
`filter: saturate(4);`

##### Default / Hover 
<img src="assets/images/bookingsubmit-default.png" alt="default booking submit button" width="147" height="46" /><img src="assets/images/bookingsubmit-hover.png" alt="hover booking submit button" width="147" height="46" />   
<img src="assets/images/contactsubmit-default.png" alt="default contact submit button" width="147" height="46" /><img src="assets/images/contactsubmit-hover.png" alt="default contact submit button" width="147" height="46" />


### Typography/Icons 

| Useage              | Source                        |
|:--------------------|:------------------------------|
| Logo Icon           | [FontAwesome](https://fontawesome.com/icons/cat?style=solid) |
| Booking button icon | [FontAwesome](https://fontawesome.com/icons/paw?style=solid) |
| Contact button icon | [FontAwesome](https://fontawesome.com/icons/envelope?style=solid) |
| Facebook icon | [FontAwesome](https://fontawesome.com/icons/facebook-f?style=brands) |
| Yelp icon | [FontAwesome](https://fontawesome.com/icons/yelp?style=brands) |
| Instagram icon | [FontAwesome](https://fontawesome.com/icons/instagram?style=brands) |
| TripAdvisor icon | [FontAwesome](https://fontawesome.com/icons/tripadvisor?style=brands) |
| Footer up icon | [FontAwesome](https://fontawesome.com/icons/angle-up?style=solid) |
| Title               | [Roboto](https://fonts.google.com/specimen/Roboto)           |
| Navigation          | [Roboto](https://fonts.google.com/specimen/Roboto)           |
| Titles              | [Roboto](https://fonts.google.com/specimen/Roboto)           |
| Content             | [Roboto](https://fonts.google.com/specimen/Roboto)           |

## Accessibility

### Alt tags
As images make up a big portion of the design of the project, I wanted to ensure the equivilent experience to someone using a screen reader was of comparable quality by providing all images with descriptive alt tags.

### Forms
Both forms featured on the site, Booking and Contact, have aria-labels so that screen readers read out what content belongs in each input field.

## Technologies Used

| Technology  | Use                             |
|:------------|:--------------------------------|
| HTML        | Content                         |
| CSS         | Styling                         |
| [Bootstrap](https://getbootstrap.com)   | Responsive structure, carousels |
| [FontAwesome](https://fontawesome.com) | Logo and Submit button icons    |
| [Google Fonts](https://fonts.google.com)| Importing of Web Fonts          |
| Git & [Github](https://github.com)| Version Control & Deployment    |


## Resources

| Resource           | Use                                       |
|:-------------------|:------------------------------------------|
| [Shoelace.io](http://shoelace.io)        | Visualising Bootstrap grids before coding |
| [Balsamiq](https://balsamiq.com)           | Wireframing                               |
| [VS Code](https://code.visualstudio.com)            | IDE and used for Git version control      |
| [Chrome Dev Tools](https://developers.google.com/web/tools/chrome-devtools)   | For debugging CSS issues                  |
| [Notion](https://www.notion.so)             | Notes & todo list, tracking progress      |
| [W3C HTML Validator](https://validator.w3.org) | Validation of HTML code                   |
| [W3C CSS Validator](https://jigsaw.w3.org/css-validator/)  | Validation of CSS code                    |

## Testing

### Validation
<a href="https://validator.w3.org"><img src="assets/images/html5-validator-badge.png" alt="w3 css validation passed" width="352" height="124" /></a> <a href="https://jigsaw.w3.org/css-validator/"><img src="assets/images/css-validator-badge.png" alt="w3 css validation passed" width="352" height="124" /></a>

### Lighthouse
<img src="https://i.imgur.com/8XWZo8D.png" alt="lighthouse score"/>  

*Performance improvements detailed in [Scope: Long Term Vision](#long-term-vision) section.*

### Bugs
After deployment, I found multiple bugs that needed addressing.

| Bug         | Fix         |
| ----------- | ----------- |
| Mobile nav didn't collapse after click      | Found the appropriate collapse class from Bootstrap documentation. **Resolved.**       |
| Links stop working after applying collapse code   | Wrapped nav items in a `<li>` as advised ([see Credits section](#credits-attributes)) **Resolved.**  |
| Footer social icons too small at mobile breakpoint | Changed font-size at various breakpoints to keep it responsive **Resolved.** |
| Gap of white space between mobile nav and hero image | Changed nav to be a fixed height and specified the top positioning to the hero image **Resolved.** |
| Indicators on carousel visible on top of mobile nav | Adjusted z-index for mobile navbar until it was on a higher level than the Bootstrap carousel indicators **Resolved.** |
| Mobile nav icon flickers when carousel slides | Changing container-fluid from 100% to 100vw resolves issue but breaks nav fixed positioning. Keeping flickering bug as it has less impact on the user experience. **Outstanding.** |



### Cross-browser Compatability
* Smooth Scrolling enabled, currently isn't supposed in Safari without additional Javascipt.

### Accessibility Testing
When the project was nearing completion, I enabled VoiceOver on my iPhone to ensure that it was able to select all of the elements without issue and that it read out the correct alt tags.

## Deployment
* I spent time studying how Git works for this project, in particular a workflow called Git Flow. This was beyond what was covered in our Code Institute module as I felt it was important to get used to the tools an everyday developer would use and I had an interest in how it worked. Rather than using GitPod, I used my own IDE and its built-in terminal to handle version control.  
* I primarily worked on the *master* branch as I knew the project wouldn't be public until I pushed it to my remote repository on Github. Ordinarily, I would have worked on a *develop* branch and only push production-ready code to *master*.  
* While working on this project, there were a few occasions where I wanted to try an implement a feature but wasn't sure the best approach. In these scenaros, I created a separate branch named after the feature and tested the code there before deciding whether I wanted to use this new method in my *master* branch.  
  * An example of this was with the hero image at the top of the site. I had created a static image, and a carousel version that scrolled through several images. I wasn't sure which would look better, on various device screen sizes, so I deployed both and spent time deciding which to use.  
  * Another example was with the booking form container. Initially this was a Bootstrap column, but it became difficult to work with at different breakpoints. I tried another way of doing this using CSS positioning and found it worked a lot better.

## Final product
Initially I had completed around 70-80% of the project by writing it in vanilla HTML and CSS, primarily using CSS grids for structure. I decided to remake the project from scratch using Bootstrap as I felt it would produce a better experience for mobile users. It was also a useful exercise as it meant I became a lot more comfortable with using Bootstrap.  
<hr>
Below are examples of how it looked vs the end product:  

<img src="assets/images/firstdraft.gif" alt="GIF demonstrating first draft"/>  

## Credits & Attributes
* All photographs taken by me
* 'About' section text taken and lightly modified from [Secret Garden Cattery](www.secretgardencattery.co.uk) (with permission)
* Bootstrap Documentation
* W3 Schools Documentation for HTML & CSS
* Carousel Source Code [here](https://www.w3schools.com/bootstrap4/bootstrap_carousel.asp)

### Code Institute Tutors/Slack
* Miklos
  * Discussed my existing knowledge of how Git works to ensure I understood it properly and if I was missing anything from its basic usage
  * I was unsure how to have a Bootstrap column push to a new line at a breakpoint, Miklos explained having a col-12 only appear at certain breakpoints will push subsequent columns to a new line.
* Tim
  * Recommended Shoelace.io to me which helps visualise Bootstrap grid's and how they look at different breakpoints
* Johann
  * I wanted to have my booking container change width at a certain breakpoint. Up until this point my booking container was a column in Bootstrap. Johann suggested it might be better to have the container be outside of a grid system and instead use positioning to determine its location at various breakpoints.
* Cormac
  * Helped me identify what elements was overflowing causing a horizontal scrollbar to appear. Talked me through ways of using Chrome Dev Tools to debug this type of issue.
* Jim Morel (JimLynx_Lead)
  * After I implemented Bootstrap's mobile navigation bar collapse-after-click code my links suddenly stopped working. Jim advised me to wrap them in a <li> to regain the functionality.

### [Back to top.](#)