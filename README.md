# Description

This is an assignment to build a responsive ecommerce web page. Nav and product container div will use flexbox. Sidebar/aside is a module that changes layout and location based on window size. Submitting the mailing list signup form results in user feedback on the page. Clicking a product's “add to cart” or “remove from cart” button updates cart count at top.

Students may use the provided mockups to guide their design to whatever extent they like. Matching the mockups is not required.

## Provided Materials

  - basic HTML and CSS
  - JSON list of products in script.js file
  - reset.css
  - images for all products
  - suggested design mockups

## Assignments

Lesson 03:

  - Make design decisions about how you'd like your site to look. You can use the provided mockups to guide your design to whatever extent you'd like- feel free to implement them exactly or make up your own design completely.
  - Code basic CSS for page. `reset.css` file should remain as it is. `main.css` file can be added to, changed, or completely redone.
  - `nav ul` and `.item-container` elements should be styled as flexbox containers. Implement a responsive grid system of your own design, or use a library, or don't use a grid at all. Be sure all important size values are proportional (em, rem, %).
  - We'll continue working on the CSS for this project throughout the course, in particular making it more responsive. The styling does not have to be perfect after this assignment. It's fine to change or add to the HTML as necessary for your styling.

Lesson 05:

  - Write a JS form handler function to be triggered on form submit. It should print to the console a friendly message that includes the value of the form element with name "email". Something like "Thanks for signing up for our mailing list, bobross@example.com!"

Lesson 06:

  - Serve appropriately sized images. Use GIMP or another photo-editing program to resize all images to more reasonable, consistent dimensions. This includes product images, the logo, and any background or other images you've included.

Lesson 07:

  - Write Javascript function that toggles the inclusion of a product in the "cart".
  - Add/edit HTML as necessary to trigger the function on click of a button for each product.

Lesson 08:

  - Write CSS that uses media queries to change layouts/style based on device size. There shoud be at least one obvious layout change in addition to elements fluidly changing width.
  - Finish styling the page.

Lesson 09:

  - Write Javascript that causes the total number of items in the cart to display next to the cart icon when that total changes.
  - Write Javascript that displays the friendly message on form submit in the page, not in the console.
  - Update the HTML and CSS as necessary to accomodate these changes.
  - Update the Testing section of this README with your own information.

*Extra Challenge*: Incorporate unit tests with [Qunit](https://qunitjs.com/).

*Extra Challenge*: Code a popup that toggles between hidden and displayed when user clicks on cart icon. It should show information about items in the cart (maybe list of their names, but up to you).

*Extra Challenge*: Serve appropriately sized images for user's device. Create multiple sizes of each image, and serve the appropriate one using the `srcset` and `sizes` attributes on the `img` tags. This will require naming all of the images consistently, e.g. "ombre-infinity400.jpg", "ombre-infinity200.jpg". [More](https://css-tricks.com/responsive-images-youre-just-changing-resolutions-use-srcset/) about [srcset](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/img)

*Extra Challenge*: Use browser storage to save details about a user's cart so when they revisit the page, it's in the same state as when they left it. [More about browser storage](https://www.w3schools.com/html/html5_webstorage.asp)

*Extra Challenge*: Dynamically generate the HTML for product listings from the JSON objects in script.js.

## Requirements

  - Site layout looks good on all sizes of devices. At a minimum, elements are proportionally styled and aside element changes location and layout at different screen sizes. This should be tested using a variety of devices and at least one online browser compatiblity testing tool.
  - Nav and product container elements are styled using flexbox.
  - Appropriately sized images are served.
  - User can add and remove items from their cart, which changes cart count number at top of page.
  - This README is updated to include information about the testing steps taken to ensure site quality.
  - Site is live on GH Pages hosting.

## Grading
Each weekly assignment will be graded independently. There will not be a final grade for the entire project.

## Testing
[update this section with information about the testing steps you took to ensure site quality]
User base for this website:
-Women ages 30 to 65 (primarily/main focus)
-Men shopping for gifts for family or friends (occasionally)
-20 to 29 year olds shopping for gifts for their family or friends (occasionally)

-->Women ages 30 to 65:
  -looking for gifts
  -looking for themselves
  -"fashionistas"
  -skiers/snowboarders
  -hikers
  
Research percentages/conclusions (research below is global)
-57% of women vs 39% of men purchase clothing/shoes online
-66% of women have smart phones-test both mobile and desktop/laptop
Age:
-83% women 30 to 49 have smart phones-test both mobile and desktop/laptop
-58% women 50 to 64 have smart phones-test both mobile and desktop/laptop
-only 30% of women 65+ have smart phones therefore they'd more likely look at website on a desktop/laptop browser
-Info found on adage.com/images/in/pdf/1114.pdf (2011 data) indicates the following:
    -Millenials online shop: use laptops 90% of the time, desktops 70% of the time, and smartphones only 18% of the time
    -Gen X online shop: use laptops 97% of the time, desktop 95%, and smartphones only 19% of the time
    -Boomers online shop: use laptops 87% of the time, desktops 75% of the time, and smartphones only 4% of the time
  -->Indicates to me that most women use laptops first, desktops second, and surprisingly smartphones last when it comes to online shopping
  -->This data has likely changed since 2011, but at this time it's the most comprehensive site I found for this specific subsect of the population.
Color preferences (in order to build the best color design):
  -35% of women selected Blue as their favorite color
  -Only 1% selected white as their favorite color, so limit white space where you can if it's something you want to focus on
  -Orange was the least popular color at 33%, followed by Brown at 20%, avoid using these colors as much as possible
  -Colors to avoid b/c they look "cheap": orange 26%, yellow 22%, brown 13%
  -In one study it showed that women gravitate towards "soft" colors, like light blues, greens, yellows, and pinks
  
Testing:
-ResponsiveDesignChecker.com:
  -First tested for responsiveness on various tablet sizes:
      -Apple iPad Mini, Amazon Kindle Fire/Fire HD, Asus Eee 1000 768x1024, site resized well into single column grid of the clothing modules, easy to read still
      -Apple iPad Pro 1366x1024, site resized well to a three/two column grid of the clothing modules.  When at this size it triggered the outlined version of the site header.  Font is easy to read at this size which is beneficial to all users, but particularly useful for 65+ users
      -Nexus 7 600x960, shrinks to one column, font is still readable
      -Nexus 9 1024x768, responsive grid shrinks to 2 columns, font still legible 
      -Samsung Galaxy Tab 10 800x1280, instead of grid responding to size of screen by shrinking to 1 column, the 2 column design as seen on the Nexus 9 just gets smaller.  Text might not be as legible for people with low vision or those who's eyesite is getting worse with age or health
      
   -Next, tested for responsiveness on desktop/notebooks:
      -24" 1920x1200 screen, site responds by having a row of 5 modules with a row of 3 modules below.  Font appears small on this site, but on work desktop, which is 1920x1080 and using Firefox, it does fill the screen and font is more legible
      -23" and 22" didn't change, both had two rows of 4 modules, font was small
      -20" 1600x900, still two rows of 4 modules, but font size increased/more legible, site header changed to outlined text
      -19" 1440x900, site width decreased causing the modules to switch to 2 rows of 3 modules, and 1 row of 2 modules.  Header remained the outline text version and font stayed same size as on 20" screen
      -15" 1366x768, same as above
      -13" 1024x800, screen width reduced causing rows to go to 4 rows of 2 modules.  Header text reverted back to solid blue text, body text is still legible.
      -10" notebook 1024x600, only difference was that screen height shrunk, otherwise body and header text remained the same.
      
  -Next, tested for responsiveness on smartphones:
      -Does not work well on iPhone 3/4/4s/5/5s, Samsung Galaxy S5/6/7, Sony Xperia Z2/Z3, Nexus 4
      -Does respond well to iPhone 6s Plus/7 Plus, Google Pixel and Nexus 5/6.  On these grid stacks as one column, header text remains dark blue w/out outline
      
  Conclusions:
  While it's important to focus on all potential customers, based on the data we're looking at a user who is between 30 and 50, primarily using a desktop/laptop.  Site should be lighter colors of blues, greens, and limited white space.  Overall the site works well, especially for this user type, but it could use some work as far as resizing for tiny/smaller screens of certain mobile phones. Will continue to work on this as site progresses.
















