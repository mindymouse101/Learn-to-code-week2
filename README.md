# Learn-to-code-week2
Last week we signed up for GitHub and edited the HTML of a website we had forked.
This week we'll be working on that same site, but this time we'll be editing the
CSS to style the site as we see fit!


##This week we're going to change the CSS on the website we created last week!
Navigate to the repository of the website that you created last week and click
on the index.html file. Lets take a minute to look through the contents of the
###Change the currently referenced stylesheet
```head``` tags.

```
<head>
    <meta charset="utf-8">
    <link href='http://fonts.googleapis.com/css?family=Source+Sans+Pro:400,700|Montserrat' rel='stylesheet' type='text/css'>
    <link rel="stylesheet" type="text/css" href="css/style2.css">
    <link rel="icon" href="favicon.png" type="image/x-icon">
    <title>Hello World</title>
</head>
```


The ```<meta>``` tag is there to let the browser know that this page is using
the utf-8 character set.

The first ```<link>``` tag is bringing in the "Montserrat" font from the free
GoogleFonts library.

The second ```<link>``` tag is referencing the CSS stylesheet that the page is
using.

The third ```<link>``` tag sets the favicon for the site.


###Change the currently referenced stylesheet
In the second ```link``` tag  you should recognize that ```href="css/style2.css"```
is just a link to our "style2.css" file. Lets change that to our plain old
"style.css" file stored in that same folder.

Click the edit button while looking at your ```index.html``` page and change the
stylesheet reference from "style2.css" to "style.css". Scroll to the bottom of the
page, leave a commit message and commit your changes.

###Change the Font to something from Google Fonts
Navigate to google fonts: https://www.google.com/fonts

1. Find a font you like and click "add to collection".

2. On the bottom right side of your screen click "use".

3. On the use page, scroll down and copy the link tag provided.

4. Replace the first link tag in your ```index.html``` file with the new link tag
you copied from google fonts.

5. Commit your changes.


###Change the font-size of your social links
First lets change the font size for all the links on the bottom of your page. In
the footer tag of your ```index.html``` file notice that the ```<ul>``` tag has
the classes "meta" and "inline-list", lets look for those classes in the
style.css file.


You'll first notice that the meta class is represented as ".meta" in the CSS
file. (I've cleaned up the CSS to make it more readable.) The "." identifies
that "meta" is a CSS class, inside the curly brackets are all the attributes
associated with that class. Change the font-size to 40px

```
.meta {
    text-transform: uppercase;
    font-family: Courier New, Quicksand, "Helvetica Neue", "Arial", sans-serif;
    font-size: 18px;
    letter-spacing: .15em;
}
```

###Add some CSS of your own.
Now that you have changed the CSS someone else has written, create some all new
CSS from scratch!

A good place to start will be changing the font color for all the links at the
bottom of the page. If you want to change the color of all the links to the same
thing you would use a class, but since we want each link to be a different color
we'll be using id's.

1. To each ```<li>``` tag ad an id tag like ```<li id="link1">```
2. In your "style.css" file add each of your new id tags:
``` #link1 {}```
3. Change the color of each id:
``` #link1 {color: red;} ```
