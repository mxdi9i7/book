# 2. HTML

### 2.1 What is HTML

#### A little history

HTML stands for Hyper Text Markup Language, it is a markup language for designing webpage structures. What is markup you ask? Well, markup language is not like programming language, programming languages will contain logic, a lot of logic. Where markup language does not care about logic. Whatever you write gets rendered by your browser and displayed on your page. There is no such thing as bug in markup languages because there is no logical expressions.

#### HTML's role in a web page

What does HTML do on a web page? Basically every thing. Everything you see on a website is marked up using HTML. Images, links, paragraphs, headers, videos, they are all written with HTML!

Think about HTML like the structures of a building, the floors, the ceiling, the walls and the doors. The building is your website.

### 2.2 HTML structures

## `<div>Hello world</div>`

This is a typical HTML tag, the &lt;div&gt;s wrapping around the words "Hello world" is the tag. There is a beginning and an ending tag

Every single HTML page needs the same boilerplate to begin with, you may add additional code to this boilerplate based on your needs, but here it comes:

```
<html>
    <head>
        <meta charset="utf-8" />
        <title>Page Title</title>
    </head>
    <body>
        <div>Hello world</div>
    </body>
</html>
```

Write the above code in your editor and you have just written your first HTML page.

#### What are those

`<!DOCTYPE html>` is the beginning tag for any HTML5 pages. HTML5 is the latest version of HTML, which comes with a lot of exciting features, for you to be able to use these features, you have to let the browser know that you're writing in HTML5 by including this tag at the top of your document.

`<html></html>` is the wrapper tag for all HTML tags, this tag wraps around all other tags from beginning to end.

`<head></head>` is the wrapper tag for HTML meta information. As you can see, the head tags are wrapping around two other tags. Every tag inside the head tag is a property/meta tag that defines the page
- **wrapper tag**: a tag that wraps around other tags
- **meta information** properties of a web page (screen ratio, foreigh character encoding, stylesheets etc.)

`<body></body>` is the wrapper tag for most HTML tags. The difference between body tag and head tag is that everything in the body tag you can visibly see (images, links, paragraphs etc.). Everything in the head tag is invisible to the web page visitor.

`<meta />` is the meta tag that defines a specific property of the web page. In this case, we are allowing foreigh characters to correctly display on our web page. More examples of meta tag usage can be found [here](/).

`<title></title>` is the tag for the title of the web page tab. Whatever you put inside of the tag will display in the tab header on a browser.

### 2.3 HTML tags and relationships

As you can see, some HTML tags are wrapping around other HTML tags and some HTML tags are being wrapped inside some other HTML tags. It all looks very confusing, but once you understand what the wrapping means and the relationships between then, the structure will all be crystal clear to you.

```
    <sometag>
        <someothertag>
        </someothertag>
    </sometag>
```
What's illustrated above is a very simple HTML structure, where sometag is wrapping around some other tag. 

In situations like this, sometag is acting as someothertag's parents. And the someothertag is sometag's children. Why is it parent but not mom or dad? Because there is an opening tag and a closing tag. Same goes for someothertag, it's the children of its parents because there is a opening tag and there is a closing tag. 

*PS: I made the last part up but that could be a good way to remember to always include a closing tag to all your tags. You woundn't want to make any tag lose one of its parents or children, would you?*

```
    <sometag>
        <someothertag>
            <yetanothertag>
            </yetanothertag>
        </someothertag>
    </sometag>
```

In a more complex example we have yetanothertag inside of someothertag. Could you guess what its relationship is with the outmost sometag? Yes, its their grandchildren. And sometag is yetanothertag's grandparents. This is as far as HTML goes in ancestry.

```
    <sometag>
        <someothertag>
        </someothertag>
        <anothertag>
        </anothertag>
    </somtag>
```

Can you guess what relationship

#### More HTML Tags

Due to the nature of this tutorial series, we are only going to go over the most popular and used tags and their usage, for a complete reference of all the HTML tags, please click [here](/).

##### --- Level 1 ---

#### `<p></p>` 
paragraph tag, most commonly used for words, sentences, labels and paragraphs. Has a small and thin font as default. Example: `<p>hello</p>`

#### `<h1></h1>` 
header tag, most commonly used for titles and subtitles. Has a large and bold font as default. Example: `<h1>World</h1>`

more examples of titles:
- `<h2></h2>`
- `<h3></h3>`
- `<h4></h4>`
- `<h5></h5>`
- `<h6></h6>`

As the number increases, the font becomes thinner and smaller

#### `<a></a>`
 anchor tag, most widely used for hyperlinks, anchor links (scroll back to top or bottom button). Needs to have an attribute of `href` to define its destination. Needs to have something in the middle to give it an appearance.

A couple things that needs addressing:
###### What is an attribute?
An attribute goes inside the beginning tag's <> signs. They define the property of your tag. For example, the `href` attribute defines the address of the link that your anchor tag points to. 

###### What does it mean to give the `<a>` tag an appearance?
Anchor tags needs not only the link url that it should point to, it should also have an appearance for users to click on. The appearance could be a link of text, an image, a container or a button.

Example of a complete anchor tag:

 `<a href="https://bctc.io">Click me</a>`

 In this example, the `href` is pointing to an address called: https://bctc.io, and the user will see it as a colored 'Click me' link. Kinda looks like this: <a href="https://bctc.io">Click Me</a>

 #### `<img />` 
 Image tag, most widely used for, well, images. Image tags needs a `src` attribute to define the address of the image resource to be displayed and optionally an `alt` attribute to define a placeholder text for people that either have a slow internet connection that can't load the picture or blind people that read a web page from a assistance device. 

 Example: 
 `<img src="https://bctc.io/logo.png" alt="this is a logo">`

##### --- Level 2 ---











