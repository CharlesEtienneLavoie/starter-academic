
# Welcome to my academic website, [celavoie.netlify.app](https://celavoie.netlify.app/)

This site was built using (and adapting) the Academic Template for [Hugo](https://github.com/gohugoio/hugo). The Hugo **Academic Resumé Template** empowers you to create your job-winning online resumé and showcase your academic publications. [**Wowchemy**](https://wowchemy.com) makes it easy to create a beautiful website for free. Edit your site in Markdown, Jupyter, or RStudio (via Blogdown), generate it with Hugo, and deploy with GitHub or Netlify. Customize anything on your site with widgets, themes, and language packs.

# So, you want to fork my site? Go ahead! But read this...

I encourage everyone and anyone to fork (copy) my site if it looks like you would want your own site. Of course, I would request to keep the site footer to acknowledge Wowchemy as the open source website builder, and well, myself as the builder of that particular version of the template!

Below, you will find detailed instructions about what to do after forking the site.

# Instructions for forking this site

## Installing the prerequisites...

1. First, you will need to [create a fork](https://docs.github.com/en/get-started/quickstart/fork-a-repo) of this repository.

1. Second, you will need to create an account at https://www.netlify.com/, click `Add a new site`, `Import an existing project`, then choose `GitHub` as provider, then pick the fork you created before.

1. There! You have your website up and running already! The URL to your new site will look something like this `yoursitename.netlify.app`. You can change the name of the subdomain (`yoursitename`, before the `.netlify`) from the Netlify site settings, but if you have your own custom domain name, you [can also change it](https://www.netlify.com/blog/2021/12/20/how-to-add-custom-domains-to-netlify-sites/). Try your new site URL in your browser to confirm it works.

1. Now it's time to make some changes, like changing the name, bio, photo, publications, etc. Exciting!! Note that is is possible to make all changes directly on github.com, but I believe it is easier to see the changes you bring to the website in real-time. Therefore, I recommend that you download [GitHub Desktop](https://desktop.github.com/), log in, and make a local copy of the fork on your computer.

1. Next, to view the website in real time, you will need to use Windows PowerShell. It is already installed with Windows, you just have to type the name in the search bar and it will pop up.

1. You will also need to install Hugo extended. [Detailed instructions](https://wowchemy.com/docs/getting-started/install-hugo-extended/#cms) are available, but in a nutshell:

> Open the Windows Powershell 5 app, installing it if necessary.
>
> Install Scoop, the package manager for Windows, by pasting the following commands into Powershell and pressing the Enter ↵ key:

```
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
iwr -useb get.scoop.sh | iex
```

> Press Y and enter if asked Do you want to change the execution policy?.
>
> Install Hugo and its dependencies:

```
scoop install git go hugo-extended nodejs
```

## Running the live server

So far, so good. Next, in Windows PowerShell, there are two commands you need to kickstart your live website preview. First, you have to change the working directory to your fork. This might look like this:

```
cd "D:\GitHub\starter-academic"
```

Second, you have to run the following code to run the hugo server that will preview your site:

```
hugo server
```

Then, open your browser to the following URL to browse your site:

```
http://localhost:1313/
```

## Personalizing your site

Nice! Now is time to have fun. Make sure to change the following:

- [ ] On the home page: your name and catchy intro sentence (beware, that part was made in custom HTML so could be confusing!)
- [ ] On the bio page: Your photo, name, title, university, social media URLs, bio, interests, education, and skills.
- [ ] On the publications page: your publications (duh!)
- [ ] On the contact page: your email, phone number, address, directions, and google maps coordinates. You can delete the picture as well.
- [ ] You can delete some sections of the website if they don't apply to you: News, Blog, Media, Tutorials, Donate, etc.
- [ ] There is still things that you don't see on the site but might want to clean anyway (more below).

Some tips:

- To change the website icon, change the photo located at `starter-academic\assets\media\icon.png`.
- To change the menu layout, change the file located at `starter-academic\config\_default\menus.toml`
- To change your contact information and social media URLs, change the file located at `starter-academic\config\_default\params.toml`
- To host files at the root of your site, place them in `starter-academic\static`. Feel free to delete all of my other files there (EXCEPT the admin folder).
- The only other place you need to know about is the one located at `starter-academic\content`. From there, choose your language (and you will need to change the files for each language individually each time), and you can start making changes to the content of your site. Each folder there represents a page on your website. Feel free to delete any and all pages that you don't want. In each of these folders, there is a `index.mdV` file. That's the file you don't usually want to change. Edit the other file instead.
- For project pages (blog, media, news, tutorials), it works a bit differently. The page has its own folders, but individual elements have their own folder too, usually called "project-media" or something like that.
- Don't forget to change your author profile in: `starter-academic\content\en\authors`.
- Redirects can be specified in `starter-academic\netlify.toml`. In that file, please delete the "Strict-Transport-Security" headers paragraph (unless you have your own Report URI account).
- Google analytics can be specified in `starter-academic\config\_default\params.toml` (please delete/replace my GA ID).
- Don't hesitate to ask me questions, or ask on the wonderful Wowchemy discord: https://discord.gg/z8wNYzb
- Make sure to read the docs first though: https://wowchemy.com/docs/

# Saying thank you

If you forked my site and enjoy it, consider [sponsoring me](https://github.com/sponsors/rempsyc) and [Geo Cushen](https://github.com/sponsors/gcushen), the creator of Wowchemy.

