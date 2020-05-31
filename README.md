# jekyll-github-starter-pack

Are you familiar with basic HTML tags? or, Markdown syntax? Can you understand extremely basic CSS entries? Are you comfortable with the GitHub web interface?

Yes?

Then come, build your own website on GitHub by using Jekyll to generate a website for you from the Liquid templating engine.

No, you don't need to know either Jekyll or Liquid to get started. Once you've taken off with this starter pack, though, you'll learn as much as you need to along the way; nothing more, nothing less.

> Why can't you just use plain HTML (or plain Markdown), CSS, JS to build your website through `gh-pages` on GitHub? You absolutely can!
> 
> But when you use `Liquid`, you can use variables that'll output their values on the page at buildtime, and you can use templates for repeated blocks of text. As an example, suppose you have a help portal where certain parts of text must change according to certain parameters, you could use `Liquid` to build your pages through `Jekyll` and then render them on GitHub (or any other host).

<hr/>

-  [Prerequisites](#prerequisites)
-  [Files and folder](#files-and-folders)
-  [First steps](#first-steps)
-  [Next steps](#next-steps)

<hr/>


## Prerequisites

This template is meant for beginners. You need have a basic knowledge of HTML, CSS, and JS.

## Files and folders

Because GitHub uses Jekyll to render pages, it's essential to use a directory structure that Jekyll understands. This template contains the barest minimum files that you need to get a website up and running.

<pre>
- _layouts        # folder to contain HTML templates
  -- default.html # file that governs the layout of pages
- css             # folder to contain stylesheets
  -- main.css     # file that governs the look and feel of pages
- topics          # folder to contain pages of the website
  -- page1.html   # a page of the website
  -- page2.md     # another page of the website
  -- page3.md     # still another page of the website
- _config.yml    # basic configuration info
- index.html     # landing page of the website
</pre>

## First steps

1. Scroll up, locate the **Use this template** button, and click it.
2. Specify a repository name. The name you choose will be used in the URL of your website, like this: `https://_yourGithubID_.github.io/_repositoryName_`.
3. Click **Create repository from template**. The files and folders from this repository are copied over to a new repository for you.
4. In the new repository you just created, locate the **Settings** button and click it. Scroll down to the section called **GitHub pages** and, in the list for **Source**, ensure that **master branch** is selected.
5. In the `_config.yml` file, put down your own name and replace the value of `baseurl` with the name of your repository. This name is the same as the one you specified in step 2 earlier.
6. Navigate to `https://_yourGithubID_.github.io/_repositoryName_`. What you see on the webpages is pretty much the same as what you saw at https://aninditabasu.github.io/jekyll-github-starter-pack. You now have a starting point to work with.
7. Return to the **Code** page on the GitHub web interface, and edit the files so that they fit your vision for your website:
   1. In the `topics` folder, edit the `.html` and `.md` files as you deem fit. Just use HTML or Markdown tags like you normally would, but retain the text of lines 1 through 4 as is. Do not touch them :slightly_smiling_face: Feel free to change anything from line 5 onwards.
   2. In the root folder, edit the `index.html` file, which is the landing page of your website, as you deem fit. Again, _do not_ touch lines 1 through 4.
6. (Optional) Delete the `LICENSE` and `README.md` files. They're nice to have for a GitHub repo but you don't really need them to get your website up and running.
7. Go to `https://_yourGithubID_.github.io/_repositoryName_`. You should now see your own content on the website.

## Next steps

1. Open a file in the `topics` folder and play with lines 1 to 4 :slightly_smiling_face: This part is called `Front Matter` in Jekyll-Liquid parlance. The `topics` > `.html` or `topics` > `.md` files in this template have only two entries for front matter:
   - `layout`, the value of which in this case is `default`. This tells the build engine to use a file called `default` from the `_layouts` folder to render the page.
   -  `title`, the value of which in this case is `page1`. This is the text that is displayed as the title on browser tabs.
   
    This front matter is actually a `YAML` code block and, for your files to render correcly, should always be placed at the very top of the file. You can specify your own variables here, and call the value of those variables on the page later. For example, you can define a variable like this: `hit_list: ['Cruella', 'Villanius', 'Voldemort']` and then pick each item from this list and use it somewhere on the page.
  
2. Edit the `_layouts` > `default.html` file to play around with the look and feel of your website. If you've renamed any of the files in the `topics` folder, remember to use those names in the `<nav>` section of the file.
> Remember, however, that your files in the `topics` folder as rendered as `.html` on your website. Therefore, even if you have a file named `page2.md`, if you're calling it (referencing it) in the `default.html` file, call it as `page2.html`.

Use the `css` folder to place your styling information. If needed, create `image` and `js` folder at the root level (the same level as `css` and `topics`) for your pictures and JavaScript files. You could, of course, have all JavaScript, images, and stylesheets right at the root level itself (instead of keeping them inside special folders), but having separate folders for them looks a bit less cluttered. 

3. Rename the `topics` and `css` folders (and `images` and `js` if you have them), and use any names for any files that you place inside these folders. Just, don't rename `_layouts` because that name is needed by the build engine. Also, do not rename either `_config.yml` or `index.html`.

As you become comfortable with these files, you can explore the Jekyll documentation for more info about what more files and folders you can put into use for your website. Here are some resources:

- Liquid [introduction](https://shopify.github.io/liquid/tags/comment/)
- Jekyll [variables](https://jekyllrb.com/docs/variables/) and [includes](https://jekyllrb.com/docs/includes/)
