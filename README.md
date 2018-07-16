# LZ-ghost

[LZ's blog](https://blog.lizen.me) theme base on [ghost-wbkd-master](https://github.com/wbkd/ghost-wbkd) for Ghost. 

Beautiful, minimal and responsive. This is the latest development version of LZ-ghost.

![screenshot-desktop](https://i.imgur.com/B2qZxfD.png)

&nbsp;

# Architecture

```
├── README.md                   # Document
├── dist                        # zip file will be here
├── package.json			    # the project document
├── src                         
│   ├── built                   # the dest of files have been compiled
│   ├── css                     
│   ├── fonts                   
│   ├── js                      
│   ├── screenshot-desktop.png  # the view of desktop
│   └── screenshot-mobile.jpg   # the view of mobile
├── partials                    
│   ├── header.hbs              # index header
│   ├── floating-header.hbs     # other header
│   ├── loop.hbs                # articles page
│   ├── navigation.hbs          # navigation
│   └── sidebar.hbs             # sidebar
├── author.hbs                  # author page
├── index.hbs                   # home page
├── default.hbs                 # the main template of blog
├── error-404.hbs               # not found page
├── error.hbs                   # error page
├── page.hbs                    # 靜態文件(Image)
├── post.hbs                    # single article page
└── tag.hbs                     # category page
```

# Development

our styles are compiled using Gulp/PostCSS to polyfill future CSS spec. You'll need Node and Gulp installed globally. After that, from the theme's root directory:

```bash
cd ${projectDir}
npm install
npm run dev
```

Now you can edit `/assets/css/` files, which will be compiled to `/assets/built/` automatically.

The `zip` Gulp task packages the theme files into `dist/<theme-name>.zip`, which you can then upload to your site.

```bash
$ npm run zip
```
---

### mobile view

![screenshot-mobile](https://i.imgur.com/ELhZQsP.jpg)

# Copyright & License

Lizen's Blog © 2018 All right Reserved.