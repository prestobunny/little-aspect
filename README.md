# Little Aspect
![Thumbnail of the theme for the Tumblr theme garden.](https://github.com/prestobunny/little-aspect/blob/master/preview/thumbnail.jpg)

A lightweight pink and purple Tumblr theme based on Zoe, the awesome-awesomest champion in League of Legends ever. It's the perfect theme if you're into vaporwave and sunset colors. [Check out the demo site!](https://littleaspecttheme.tumblr.com/)

Little Aspect has a chunky pink left-hand sidebar on wide screens which moves to the top of the page on smaller screens.

## Features
- Supports all post types
- Clean and legible code
- Accessibility-ready to the best of my ability!

Aspect of Twilight not included.

## Screenshots
<img alt="A screenshot of Little Aspect showing the sidebar-content layout" src="https://github.com/prestobunny/little-aspect/blob/master/preview/screenshot1.jpg" width="300" style="float:left;" />

<img alt="A screenshot of Little Aspect showing the full-width layout for smaller screens." src="https://github.com/prestobunny/little-aspect/blob/master/preview/screenshot2.jpg" width="300" />

## Notes
### Be careful minifying the HTML
Post dates and pagination are coded into the theme using Tumblr's variables. Auto-minifying the script will strip the spaces between them and smash them all together.

### What the inline script does
The Javascript at the bottom of the page template serves two functions: first it attempts to find photosets with individually captioned photos in order to assign each of their figcaptions an ID based on the associated source image url (since Tumblr provides no variables with which to do this). This is so the theme can add an aria-labelledby attribute to each image associating them with their captions, in order for photosets to conform to the [WCAG 2.0 best practices outlined here](https://www.w3.org/WAI/tutorials/images/groups/#a-collection-of-images).

The second part of the code looks for notes on permalink pages that are from the author of the current blog and assigns them a special class, "note-thisblog". If you look at the demo site, you can see that notes from the blog author are emphasized.

## Changelog
### 1.0.0
Initial release

## License
Little Aspect theme code is released under the MIT license. Basically do whatever you want with it. The two glitter images used in post headers/footers are public domain.

The "like" and "reblog" icon SVGs used in the post actions bar and next to permalink page notes belong to Tumblr.

Any content used on the demo site belongs to its respective owners.
