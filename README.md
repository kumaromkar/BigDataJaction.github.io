# BigDataJaction.github.io
## Setup:

1. Download and install git 
2. git setup 
    ```bash
    git config --global user.name "your name"
    ```
    ```bash
    git config --global user.email youremail@gmail.com
    ```

3. Clone the repo
    ```bash
    git clone https://github.com/bigdatajunction/bigdatajunction.github.io.git
    ```

4. go to the folder 
    ```shell
    cd bigdatajunction.github.io
    ```
5. install  hugo 

    mac:
    ```bash 
    brew install hugo
    
    hugo version

    ```
    windows:
    ```bash 
    choco install hugo
    ```

6. theme setup:
    ```bash 
    git rm -r --cached themes/ananke
    ```
    <!-- ```rm -rf themes/ananke``` -->
    delete contents of .gitmodules 
    ```bash
    git submodule update
    ```

    Install Anakle theme into project  
    ```bash 
    git submodule add https://github.com/theNewDynamic/gohugo-theme-ananke.git themes/ananke
    ```

7. Start Hugo Server / build drafts and run with -D
    ```bash 
    hugo server -D
    ```

8. Create a hugo page/blog
    ```bash 
    hugo new posts/my-first-post.md
    ```

    ```bash 
    Content "\\content\\posts\\my-first-post.md" created
    ```
--------------------------------------------------------------------------
## To cerate a blog 
```bash 
hugo new posts/post_name.md
```

Edit the blog-uri.md file from location 
```nash 
content\\posts\\blog-uri.md
```

Don't forget to make draft == false in .md file.
```md
draft: false
# means blog is ready to be published
```

--------------------------------------------------------------------------


## workflow

1. git checkout dev

```kumarom@KUMARs-Air-2 bigdatajunction.github.io % git checkout dev
M       README.md
Already on 'dev'
Your branch is ahead of 'origin/dev' by 1 commit.
  (use "git push" to publish your local commits)```

2.  Create blog

Create your First Chapter Page
Chapters are meant to be top level pages that contain other child pages. They have a special layout style and often just contain the title and a brief abstract of the section.

Now create your first chapter page with the following command:


```
hugo new --kind chapter basics/_index.md
```

When opening the newly created file content/basics/_index.md, you should see the weight frontmatter with a number. This will be used to generate the subtitle of the chapter page, and should be set to a consecutive value starting at 1 for each chapter level.

Create your First Content Pages
Then create content pages inside the previously created chapter. Here are three ways to create content in the chapter:

```
hugo new basics/first-content/_index.md
hugo new basics/second-content/index.md
hugo new basics/third-content.md
```

Feel free to edit those files by adding some sample content and replacing the title value in the beginning of the files.


```https://mcshelby.github.io/hugo-theme-relearn/basics/branding/index.html```

3. Run the local server and test the blog.

    ```bash 
    hugo server -D
    ```

4. git add and commit

```git status ```

4.1 git add file_name

4.2 git commit -m "msg"


5. Push to dev branch in remote(origin) repo.

```git push origin dev```

6. Only for omkar

Merge dev branch to local main branch

```git checkout main```


```git merge dev```

esc 
:q! + enter


Run the local server and test the blog.

    ```bash 
    hugo server -D
    ```

7. Push to remote main branch

```git push origin main```


## Final deployment 

url
```https://gohugo.io/hosting-and-deployment/hosting-on-github/```


if not auto deployed:
```md
Github repo--> Action --> Deploy bigdatajunction.. --> Run WorkFlow
```


# bencuan's notes

Hi there! Seems like you stumbled upon my archive of course notes! 

Over the years, I've found that the most effective way for me to learn and process information was to teach it. Since this isn't always practical or possible, I've ended up creating these production-quality notes as an alternative.

Although many courses at Berkeley (especially CS courses) have excellent materials and often already have a full set of course notes, I've found that many students- myself included- often struggle to process information when it's that dense. My hope is that these notes can serve as a secondary, lighter perspective on things. 

Here, you'll find a wide variety of content from basic concepts, practice problems, and example algorithm walkthroughs. Since they were all made at various times over 4 years, the quality and style may be wildly different from page to page. I intend to go through these notes and resolve any inconsistencies over (a long period of) time.

## Index

Here are the courses that I currently have notes available for, and their statuses:

 - [CS 61B: Data Structures and Algorithms](https://notes.bencuan.me/cs61b/): full guide available for all course content, based on the Spring 2020 offering
 - [CS 70: Discrete Math](https://notes.bencuan.me/cs70/): full guide available for discrete math; partial index available for probability. Based on the Fall 2020 offering
 - [CS 186: Intro to Databases](https://notes.bencuan.me/cs186/): full guide available for all topics except NoSQL and FD's/Normalization. Based on the Fall 2022 offering
 - [CS 162: Operating Systems](https://notes.bencuan.me/cs162/): course notes available for most topics. Based on the Fall 2021 offering
 - [CS 168: Intro to the Internet](https://notes.bencuan.me/cs168/): course notes available for most topics. Based on the Fall 2022 offering
 - [CS 61A: Structure and Interpretation of Computer Programs](https://notes.bencuan.me/cs61a/): resource index and meta-guide available. No course notes.
 - [Data 102: Data, Inference, Decisions](https://notes.bencuan.me/data102/): course notes available for most topics. Based on the Fall 2022 offering

Although I have personal notes for many other classes, they do not meet my quality standards for making them public at this time. If I have time at some point in the distant future, they may make an appearance, but don't count on this happening anytime soon.

If you made your own notes/resources for a CS, Data Science, or EE course and would like me to put a link to them here, let me know ([contributing](https://notes.bencuan.me/contributing))!

## About this website

My notes are hosted on [Netlify](https://www.netlify.com/) and are built on my custom [Amethyst theme](https://github.com/64bitpandas/amethyst) for [Hugo](https://https://gohugo.io/). You can view the source code [here](https://github.com/64bitpandas/notes).

All of the notes here are formatted in Markdown, and the majority was created using [Obsidian](https://obsidian.md/). These notes are a small fraction of my Obsidian vault; I intend to publish other small bits of it in various places such as my [blog](https://blog.bencuan.me), [devlog](https://devlog.bencuan.me), or [mastodon](https://hachyderm.io/@bencuan) if you're curious.

If you're interested in contributing, take a look at the [contribution guide](https://notes.bencuan.me/contributing).

## Contact me

Want to chat with me about these notes, or something else? You can find my contact info [here](https://bencuan.me/contact).# BigDataJaction.github.io
