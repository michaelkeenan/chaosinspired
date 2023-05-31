# Chaos Inspired

## How to add artworks

### Adding files to GitHub

This section will describe how to add files directly to the website in GitHub from GitHub's web app, which you'll use to add artworks to the website. Programmers use more complicated systems for adding files to GitHub, so beware of that in case you end up googling (or asking an LLM) for help with this, and don't get sidetracked by methods that aren't about the GitHub web app.

From the web app, there are two ways to add a file. You can upload a file directly, which you'll use for uploading images, or you can create files and edit them in GitHub's text editor, which you'll probably use for entering details about artworks (like titles and descriptions and Shopify IDs and so on).

Projects in GitHub are called repositories. Repositories are primarily just to store files and track their changes over time. In our case, GitHub is also using the repository to generate the files for the website, so when you add files to the repository, they appear on the website (which takes a couple of minutes, during which GitHub recompiles the site and runs some tests).

To *upload* a file, go to a directory in the repository, e.g. the [artworks directory](https://github.com/michaelkeenan/chaosinspired/tree/main/images/artworks). There should be an Add File button in the top right. (If there isn't, the problem is probably that you're not logged in, or that you don't have write access to the repository.) It's a dropdown button, so select Upload Files. Add the files to the file selection box, and write a brief description of what you did in the Commit Changes section, e.g. "Add images for Wings And Dirt 2: Dirtier and Wingier".

To *create* a file in the text editor, go to the directory you want to create the file in, e.g. the [_gallery directory](https://github.com/michaelkeenan/chaosinspired/tree/main/_gallery). Click Add File in the top right, and select Create New File from the dropdown. Type the file content in the main text editor box, and name the file in the textbox in the top left. When you're finished, click Commit Change in the top right. (If the button is disabled, it's probably because you haven't yet entered the filename in the filename textbox.) Clicking Commit Change will open a window where you're prompted for a Commit Message. Write a brief description of what you did, e.g. "Add metadata file for Wings And Dirt 3: Wings, Dirt, and Blood".

### Entering the details of the artwork

To add an artwork, first upload its images to /images/artworks/. (We do that first, because the next step will cause the artwork to appear on the site, so there'd be broken images if you did the next step first.)

Next, create a file in the /_gallery folder (note the preceding underscore character), with a name like artwork-name.md. The filename will affect the URL, so keep it URL-friendly. (To keep it URL-friendly, avoid spaces and most special characters, and use hyphens to delimit words. Best to only use alphabet characters, numerals, and hyphens.) (The .md extension won't be part of the URL; it just indicates that it's a Markdown file.) You'll probably want to just copy another artwork's file and use that as a template, changing the details. Or you could use the following template. Make sure to include the line with three hyphens at the beginning, and the similar line at the end. (If you're viewing the raw text of this file, rather than interpreted Markdown, then you'll also see three backticks/left-quotes around the template. Those are *not* part of the template; don't copy them too.)

```
---
layout: artwork
title: Artwork Title Here
description: Words to describe the artwork here. They'll be displayed at the top of the page.
shopify_id: 123456789 (a number corresponding to the artwork in Shopify. Including this is optional. If it's not included, there will be no Shopify Buy Now section on the page.)
front_image: image.jpg (the filename of the image that you want to be the main image for this artwork—the one that will be displayed in the front page gallery, or on the blog. This file should be placed in /images/artworks/.)
images:
- another_image_1.jpg
- another_image_2.jpg
- another_image_3.jpg
- another_image_4.jpg (these images will be displayed on the artwork's own page. Like the front image, the corresponding files should be in /images/artworks. You can enter any number of images in this list; it doesn't have to be just four files.)
---
```

To find out the Shopify ID, go to the corresponding product in Shopify Admin. The ID will be the last number in the URL, e.g. it's 8289665351971 for Brave New 1984 at https://admin.shopify.com/store/chaos-inspired-3708/products/8289665351971

### Asking an LLM for help

Of course, you can ask Keenan if you run into trouble, but if I'm not around, ChatGPT and Claude and others can probably help. The context you'd need to explain to an LLM are that you're editing a *Jekyll* site, using *Markdown* files, via the *GitHub web app*, and the website is hosted with *GitHub Pages*.

` `  
` `  

**The original README for the Clancy Jekyll theme follows:**

` `  
` `  

---
---
---



` `  
` `  
 

# Clancy is an elegant portfolio theme for Jekyll

Clancy is an elegant portfolio theme for Jekyll designed for photographers, designers, illustrators, artists, creatives, etc. This theme will help you professionally introduce yourself to your visitors and showcase your work in a minimalistic style. This super clean and fully optimized theme can be easily customized to suit your needs.

* * *

### Demo

Check the theme in action [Live Demo](https://clancy.netlify.app/) |
[Artem Sheludko](https://jekyllthemes.io/developers/artem-sheludko)

* * *

### Theme features

- Works with GitHub Pages (host it for free)
- Dark and light mode user can select themself
- 100% responsive Design
- Clean and Modern Code
- Optimized for mobile devices
- Super fast performance ⚡⚡⚡
- No jQuery, only vanilla JS
- Social sharing buttons
- Scroll to top button
- Syntax highlighting (supports the Jekyll syntax highlighter)
- Compatible with modern browsers
- Medium style image zoom
- Image Lazy loading
- Image gallery
- Tags Page
- Custom logo support
- Supports contact form (Formspree)
- Supports MailChimp newsletter
- Supports Disqus comments
- Supports Google Analytics
- Ionicons icons
- Free Google Fonts
- Free Updates & Support

* * *

### Installation

#### Installing Ruby & Jekyll

If this is your first time using Jekyll, please follow the [Jekyll docs](https://jekyllrb.com/docs/installation/) and make sure your local environment (including Ruby) is setup correctly.

* * *

### Deployment

To run the theme locally, navigate to the theme directory and run `bundle install` to install the dependencies, then run `jekyll serve` or `bundle exec jekyll serve` to start the Jekyll server.

I would recommend checking the [Deployment Methods](https://jekyllrb.com/docs/deployment-methods/) page on Jekyll website.

* * *

### Documentation

Before using the Clancy theme, please read the attached documentation.

* * *

### Support

<p>If you have any questions, please feel free to contact me by mail <a href="mailto:hi.artemsheludko@gmail.com">Contact</a><p>