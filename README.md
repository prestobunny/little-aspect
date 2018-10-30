# Little Aspect
A lightweight pink and purple Tumblr theme based on Zoe, the awesome-awesomest champion in League of Legends ever. It's the perfect theme if you're into vaporwave and sunset colors. Check it out!

https://littleaspecttheme.tumblr.com/

Little Aspect has a chunky pink left-hand sidebar on wide screens which moves to the top of the page on smaller screens.

## Features
- Supports all post types
- Clean and legible code
- Accessibility-ready to the best of my ability!

Aspect of Twilight not included.

## Notes
### How to hide the theme credit
```css
.footer__credits {
    display: none;
}
```

### Be careful minifying the HTML
Post dates and pagination are coded into the theme using Tumblr's variables. Auto-minifying the script will strip the spaces between them and smash them all together.

### What the inline script does
The Javascript at the bottom of the page template serves two functions: first it attempts to find photosets with individually captioned photos in order to assign each of their figcaptions an ID based on the associated source image url (since Tumblr provides no variables with which to do this). This is so the theme can add an aria-labelledby attribute to each image associating them with their captions, in order for photosets to conform to the [WCAG 2.0 best practices outlined here](https://www.w3.org/WAI/tutorials/images/groups/#a-collection-of-images).

The second part of the code looks for notes on permalink pages that are from the author of the current blog and assigns them a special class, "note-thisblog". If you look at the demo site, you can see that notes from the blog author are emphasized.

## Changelog
### 1.0.0
Initial release

### 1.0.1
#### New Options
- Use your global header image as the sidebar/header background
- Show a search form in the sidebar/header
- Show links to your blog's Archive, RSS, and a random post
- Change the post navigation header text
#### General Fixes
- Post pagination works better now!
- Added theme credit to html
- Wrapped theme meta tags
- Default copyright text is now blank since the {Title} tag wasn't working correctly
- Added H1 hideme class on Permalink pages to the unused main heading
- Post date/notes display has a minimum width in case lots of tags are used, and both date/notes and tags stretch to 100% width on small screens
#### Post Navigation
- Made the "Travel in Time" text customizable
- Removed future/past text
- Added arrows to jump to first and last pages
- Only page number links (not arrows) show visited styles now
- Changed the styles for the current page number
#### Photos
- Added photo__fig and photo__img classes to Photo posts
- Changed photoset__img class in Photoset posts to photoset__fig and added photoset__img to the inner img elements instead
- Centered photo elements that are smaller than the post width

## License
Little Aspect theme code is released under the MIT license. Basically do whatever you want with it. The two glitter images used in post headers/footers are public domain. The "like" and "reblog" icon SVGs used in the post actions bar and next to permalink page notes belong to Tumblr.