“[#lang racket]”
“[(define (in-dbs k n)]”
“[(letrec ([a (make-vector (* k n) 0)]]”
“[[init empty-sequence]]”
“[[seq (λ (t p)]”
“[(when (and (> t n) (= 0 (modulo n p)))]”
“[(set! init (sequence-append init (in-vector (vector-copy a 1 (add1 p))))))]”
  “[(unless (> t n)]”
“[(vector-set! a t (vector-ref a (- t p)))]”
“[(set! init (seq (add1 t) p))]”
 “[ (for ([j (in-range (add1 (vector-ref a (- t p))) k)])]”
“[(vector-set! a t j)]”
“[(set! init (seq (add1 t) t))))]”
 “[ init)])]”
“[(seq 1 1)))]”
“[(for/list ([b (in-dbs 10 4)]) b)]”
“[@477447]”
"[(*)]"
(*)

“[(for/list ([b (in-dbs 10 4)]) b)]”
		“[@477447]”
		"[(*)]"

(*)

# "[(for/list ([b (in-dbs 10 4)]) b)]" "[@477447]" "[(*)]"
# (*)
# (*)
(*)
(*)
Markdown is a lightweight and easy-to-use syntax for styling all forms of writing on the GitHub platform.
What you will learn:
•	How the Markdown format makes styled collaborative editing easy
•	How Markdown differs from traditional formatting approaches
•	How to use Markdown to format text
•	How to leverage GitHub’s automatic Markdown rendering
•	How to apply GitHub’s unique Markdown extensions
What is Markdown?
Markdown is a way to style text on the web. You control the display of the document; formatting words as bold or italic, adding images, and creating lists are just a few of the things we can do with Markdown. Mostly, Markdown is just regular text with a few non-alphabetic characters thrown in, like # or *.
You can use Markdown most places around GitHub:
•	Gists
•	Comments in Issues and Pull Requests
•	Files with the .md or .markdown extension
For more information, see “Writing on GitHub” in the GitHub Help.
Examples
•	Text
 
•	Lists
 
•	Images
 
•	Headers & Quotes
 
•	Code
 
•	Extras
It's very easy to make some words **bold** and other words *italic* with Markdown. You can even [link to Google!](http://google.com)
It's very easy to make some words bold and other words italic with Markdown. You can even link to Google!
Syntax guide
Here’s an overview of Markdown syntax that you can use anywhere on GitHub.com or in your own text files.
Headers
# This is an <h1> tag
## This is an <h2> tag
###### This is an <h6> tag
Emphasis
*This text will be italic*
_This will also be italic_

**This text will be bold**
__This will also be bold__

_You **can** combine them_
Lists
Unordered
* Item 1
* Item 2
  * Item 2a
  * Item 2b
Ordered
1. Item 1
1. Item 2
1. Item 3
   1. Item 3a
   1. Item 3b
Images
![GitHub Logo](/images/logo.png)
Format: ![Alt Text](url)
Links
http://github.com - automatic!
[GitHub](http://github.com)
Blockquotes
As Kanye West said:

> We're living the future so
> the present is our past.
Inline code
I think you should use an
`<addr>` element here instead.
GitHub Flavored Markdown
GitHub.com uses its own version of the Markdown syntax that provides an additional set of useful features, many of which make it easier to work with content on GitHub.com.
Note that some features of GitHub Flavored Markdown are only available in the descriptions and comments of Issues and Pull Requests. These include @mentions as well as references to SHA-1 hashes, Issues, and Pull Requests. Task Lists are also available in Gist comments and in Gist Markdown files.
Syntax highlighting
Here’s an example of how you can use syntax highlighting with GitHub Flavored Markdown:
```javascript
function fancyAlert(arg) {
  if(arg) {
    $.facebox({div:'#foo'})
  }
}
```
You can also simply indent your code by four spaces:
    function fancyAlert(arg) {
      if(arg) {
        $.facebox({div:'#foo'})
      }
    }
Here’s an example of Python code without syntax highlighting:
def foo():
    if not bar:
        return True
Task Lists
- [x] @mentions, #refs, [links](), **formatting**, and <del>tags</del> supported
- [x] list syntax required (any unordered or ordered list supported)
- [x] this is a complete item
- [ ] this is an incomplete item
If you include a task list in the first comment of an Issue, you will get a handy progress indicator in your issue list. It also works in Pull Requests!
Tables
You can create tables by assembling a list of words and dividing them with hyphens - (for the first row), and then separating each column with a pipe |:
First Header | Second Header
------------ | -------------
Content from cell 1 | Content from cell 2
Content in the first column | Content in the second column
Would become:
First Header	Second Header
Content from cell 1	Content from cell 2
Content in the first column	Content in the second column
SHA references
Any reference to a commit’s SHA-1 hash will be automatically converted into a link to that commit on GitHub.
16c999e8c71134401a78d4d46435517b2271d6ac
mojombo@16c999e8c71134401a78d4d46435517b2271d6ac
mojombo/github-flavored-markdown@16c999e8c71134401a78d4d46435517b2271d6ac
Issue references within a repository
Any number that refers to an Issue or Pull Request will be automatically converted into a link.
#1
mojombo#1
mojombo/github-flavored-markdown#1
Username @mentions
Typing an @ symbol, followed by a username, will notify that person to come and view the comment. This is called an “@mention”, because you’re mentioningthe individual. You can also @mention teams within an organization.
Automatic linking for URLs
Any URL (like http://www.github.com/) will be automatically converted into a clickable link.
Strikethrough
Any word wrapped with two tildes (like ~~this~~) will appear crossed out.
Emoji
GitHub supports emoji!      
To see a list of every image we support, check out the Emoji Cheat Sheet.



(*)

language: ruby
rvm:
- 2.1
script: "bundle exec jekyll build"



to improve the smell of code
to improve progress
 
Using emoji
You can add emoji to your writing by typing :EMOJICODE:.
@octocat :+1: This PR looks great - it's ready to merge! :shipit:
(*)
(*)
(*)

Viewing Jekyll build error messages
You can view Jekyll build error messages by email, in your repository, on the command line, or with a third-party service that displays error messages after each commit.
There are two main types of Jekyll build error messages.
"Page build warning" - Your build completed just fine, but there's something we think you ought to know.
"Page build failed" - Your build failed to complete. If we are able to detect the specific error, we will send you a descriptive error message with a link to supporting documentation. If we are not able to detect a specific error with your page build failure, then you will receive a generic "page build failed" error message.
Viewing Jekyll build error messages by email
You can view all Jekyll build error messages by email if you have your email set up. To add a new email address or verify an old email, see "Changing your primary email address."
Viewing Jekyll build failure messages in your repository
You can view Jekyll build failure messages in the repository settings of your GitHub Pages site.
1.	On GitHub, navigate to the main page of the repository.
2.	 
Under your repository name, click  Settings.
3.	 
Under GitHub Pages you can see current Jekyll build failure messages.
Note: Page build warnings will not display in your repository settings.
Viewing Jekyll build error messages in the command line
Tip: We strongly recommend running Jekyll locally so you can easily debug and fix build errors before pushing to GitHub. To learn more about troubleshooting options, see "Troubleshooting GitHub Pages builds."
To view all Jekyll build error messages on the command line, you must set up your Jekyll site locally on your computer, see "Setting up your GitHub Pages site locally with Jekyll" for more details. If your page isn't building after you push to GitHub, see "Troubleshooting GitHub Pages builds".
Configuring a third-party service to display Jekyll build error messages
You can configure a third-party service such as Travis CI to display error messages after each commit.
•	Add a file named Gemfile (note that the "G" must be capitalized) to the root of your GitHub Pages repository with the following content:
source 'https://rubygems.org'

gem 'github-pages'
•	Configure your GitHub Pages repository for the testing service of your choice. To set up Travis CI, for example, add a file named .travis.yml to the root of your GitHub Pages repository with the following content:
language: ruby
rvm:
- 2.1
script: "bundle exec jekyll build"
•	You may need to activate your GitHub Pages repository within the third-party testing service. For Travis, do this on your Travis CI profile page.
If you have vendored your gems into a vendor folder (or a CI service like Travis has done it for you), be sure to add exclude: ["vendor"] to your _config.yml file to avoid potential conflicts.


(*)
source 'https://rubygems.org'

gem 'github-pages'

For example, Travis CI's documentation suggests adding the following lines to a .travis.yml file:
branches:
  only:
    - gh-pages

git-commit


Because a branch in Git is actually a simple file that contains the 40 character SHA-1 checksum of
the commit it points to branches are cheap to create and destroy. Creating a new branch is as guick
and simple as writing 41 bytes to a file(40 characters and a newline)

(*)
(*)
Collaborating with issues and pull requests / About pull requests
 
Конец формы
About pull requests
Pull requests let you tell others about changes you've pushed to a branch in a repository on GitHub. Once a pull request is opened, you can discuss and review the potential changes with collaborators and add follow-up commits before your changes are merged into the base branch.
Note: When working with pull requests, keep the following in mind:
•	If you're working in the shared repository model, we recommend that you use a topic branch for your pull request. While you can send pull requests from any branch or commit, with a topic branch you can push follow-up commits if you need to update your proposed changes.
•	When pushing commits to a pull request, don't force push. Force pushing can corrupt your pull request.
After initializing a pull request, you'll see a review page that shows a high-level overview of the changes between your branch (the compare branch) and the repository's base branch. You can add a summary of the proposed changes, review the changes made by commits, add labels, milestones, and assignees, and @mention individual contributors or teams. For more information, see "Creating a pull request."

(*)

Customizing GitHub Pages / Adding a Jekyll theme to your GitHub Pages site with the Jekyll Theme Chooser
 
Adding a Jekyll theme to your GitHub Pages site with the Jekyll Theme Chooser
You can use the Jekyll Theme Chooser to create a GitHub Pages site, or to change the theme of your existing GitHub Pages site.
You can also add a Jekyll theme to your GitHub Pages site manually, by editing your site's _config.ymlfile. For more information, see "About Jekyll themes on GitHub."
1.	If you don't already have a repository for your GitHub Pages site, create a new repository with a README. Your new repository can be public or private. If your repository is private, your published site will still be public.
Tip: To create a User or Organization GitHub Pages site, you must name your repository<username>.github.io , using the name of the user or organization that owns the repository. If you choose a different repository name, then the Jekyll Theme Chooser automatically creates a Project Pages site for you. For more information, see "User, Organization and Project Pages."
2.	Navigate to your GitHub Pages site's repository.
3.	 
Under your repository name, click  Settings.
4.	On the settings page, scroll down and under "GitHub Pages":
o	 
Click Choose a theme to add a theme to your site for the first time.
o	 
Click Change theme to change an existing theme for your site.
5.	 
On the theme selection page, review your theme options. To choose a theme, click the theme you want and then click Select theme.
6.	 
If you're creating a new GitHub Pages site, you'll be prompted to edit your site's README.md file. Click Cancel to edit it later. If you'd like to edit it now, see "Editing files in your repository" and commit your changes to the master branch.
7.	 
Under your repository name, click  Settings.
8.	 
To preview your site, under "GitHub Pages" click the URL to your GitHub Pages site. For troubleshooting help, see "Troubleshooting GitHub Pages builds."
Further customizing your Jekyll site
If you'd like to change the CSS or HTML layout of your Jekyll theme, see "Customizing CSS and HTML in your Jekyll theme."
Adding more pages to your site
To learn more about adding other pages or posts to your GitHub Pages site, see Jekyll's official documentation on creating pages or posts. Other pages or posts you add to your site will share your Jekyll theme's style and layout.
Customizing your site's URL
To learn more about customizing your site's URL, see "Using a custom domain with GitHub Pages."
Choosing a different publishing source or branch
If you would like to publish your GitHub Pages site using the gh-pages branch or from a docs folder in your repository, see "Configuring a publishing source for GitHub Pages."
Further reading
•	"About Jekyll themes on GitHub"
•	Jekyll's official documentation on Themes
•	"Customizing GitHub Pages"
•	"Customizing CSS and HTML in your Jekyll theme"
•	"Editing files in your repository"
•	"Adding a Jekyll theme to your GitHub Pages site"
(*)
	

# Settings
# Change the theme

Fighting against scammers and intrubers last month from my site stole the money that l had to get for their deposits l would like
to know it will happen again or not the support service is working intermittently maybe l'm wrong but there is such an opinion
(*)


# Relative links and image paths in README files
You can define relative links and image paths in your rendered files to help readers navigate to other files in your repository.
A relative link is a link that is relative to the current file [Contribution guidelines for this project](docs/CONTRIBUTING.md)



  

