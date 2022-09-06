# Sass-project

Here I was practicing using Sass. I used the variables function for my color palette, that way if I wanted to change colors at any time, I could just change the variable
in one place.
I divided the scss into modules relevant to the layout of the page.
I started working with one file that I then split into two more sections, a header and footer. That left the original section with very little css in it, as my
website is very small and has little content on it, but I can see this being brilliant when working with a lot of css.

I used nesting to group together related code. I liked the clean look it gave and it felt very intuitive to use, but I did run into a problem placing
elements in the correct nesting order. I spent a good 20 mins scratching my head over why the css wasn't responding correctly, and it was because I nested a piece
of code under the wrong parent. I probably would avoid making really large nesting sections in the future, as I can imagine they can start to be confusing
to work with.

I wanted the two sections of the site to have the same dimensions, so I created a mixin for that. Originally I had the mixin in the main file with the header/footer
files linked, but that didn't work. Smári told me I would have to link it the other way around and that would created a weird loop causing a lot of problems.
Normally you would make a seperate file for your mixins and then link it to the other files but since I only was working with this one mixin it felt a bit weird
to add a whole file just for one piece of code. In the end I added the mixin to both the header and footer files, it feels a bit inefficient but I think it made the
most sense for a small project like this.

Finally I used the Extend function to copy the style of my "main-text" to my "bottom-text".
