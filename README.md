# jekyll-github-starter-pack

Are you familiar with basic HTML tags? Can you understand extremely basic CSS entries? Are you comfortable with the GitHub web interface?

Yes?

Then come, build your own website on GitHub by using Jekyll to generate a website for you from the Liquid templating engine.

No, you don't need to know either Jekyll or Liquid to get started. Once you've taken off with this starter pack, though, you'll learn as much as you need to along the way; nothing more, nothing less.

> Why can't you just use plain HTML, CSS, JS to build your website through gh-pages on GitHub? You absolutely can!
> 
> But when you use `Liquid`, you can use variables that'll output their values on the page at buildtime, and you can use templates for repeated blocks of text. As an example, suppose you have a help portal where certain parts of text must change according to certain parameters, you could use `Liquid` to build your pages through `Jekyll` and then render them on GitHub (or any other host).

## First steps

1. Scroll up, locate the **Use this template** button, and click it.
2. Specify a repository name. The name you choose will be used in the URL of your website, like this: `https://_yourGithubID_.github.io/_repositoryName_`.
3. Click **Create repository from template**. The files and folders from this repository are copied over to a new repository for you.
4. In the new repository you just created, locate the **Settings** button and click it. Scroll down to the section called **GitHub pages** and, in the list for **Source**, ensure that **master branch** is selected.
5. Navigate to `https://_yourGithubID_.github.io/_repositoryName_`. What you see on the webpages is pretty much the same as what you saw at https://aninditabasu.github.io/jekyll-github-starter-pack. You now have a starting point to work with.
5. Return to the **Code** page on the GitHub web interface, and edit the files so that they fit your vision for your website:
   1. In the `_config.yml` file, put down your own name and replace the value of `baseurl` with the name of your repository. This name is the same as the one you specified in step 2 earlier.
   2. In the `topics` folder, edit the `.html` as you deem fit. Just use HTML tags like you normally would, but retain the text of lines 1 through 4 as is. Do not touch them :slightly_smiling_face: Feel free to change anything from line 5 onwards.
   3. In the root folder, edit the `index.html` file, which is the landing page of your website, as you deem fit. Again, _do not_ touch lines 1 through 4.
6. Go to `https://_yourGithubID_.github.io/_repositoryName_`. You should now see your own content on the website.

## Files and folders

Because GitHub uses Jekyll to render pages, it's essential to use a directory structure that Jekyll understands. This template contains the barest minimum files that you need to get a website up and running.

<pre>
- _layouts        # folder to contain HTML templates
  -- default.html
- css             # folder to contain stylesheets
  -- main.css
- topics          # folder to contain pages of the website
  -- page1.html
  -- page2.html
  -- page3.html
- _config.yml    # basic configuration info
- index.html     # landing page of the website
</pre>

As you become comfortable with these files, you can explore the Jekyll documentation for more info about what more files and folders you can put into use for your website.

## Resources

- Liquid [introduction](https://shopify.github.io/liquid/tags/comment/)
- Jekyll [variables](https://jekyllrb.com/docs/variables/) and [includes](https://jekyllrb.com/docs/includes/)
