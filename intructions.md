Bootstrap

Initial Set-up
When starting to build you project, you need to go to the Bootstrap website and link it to your html.

On your terminal, you need to "npm init"
Next, npm i date-fns (this is optional)
Next, npm install bootstrap
Next, npm install lite server " npm install lite-server --save-dev " (not of production use)
---on your package.json file, do this
  "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1",
    "start": "npm run lite", (this must me added)
    "lite": "lite-server" (this must be added)
  },

To use Git and GitHub
  1) git init
  2) git add .
  3) git commit -m " the name of what you call your commit"
  (the succeeding commits, you just need 2 and 3)
  4) git status (use this to check your repository status)
  ** git log --online ()
  Using Remote Repository
  (source: https://docs.github.com/en/get-started/getting-started-with-git/about-remote-repositories)
  1) on GitHub, create a repository your want to link your VSC
  2) git remote add origin <your remote repository URL> (you can either push using either two URL a) HTTPS or b) SSH)
  (use " git remote set-url origin <URL> " to change your URL)
  (source: https://docs.github.com/en/get-started/getting-started-with-git/managing-remote-repositories)
  ( " git remote -v " is to verify your remote repository address)
  3) git push origin main (main can be changed to whatever destination--when all is set all you have to do is just "git push")

What is The Viewport? (Source: https://www.w3schools.com/css/css_rwd_viewport.asp )
The viewport is the user's visible area of a web page.

The viewport varies with the device, and will be smaller on a mobile phone than on a computer screen.

Before tablets and mobile phones, web pages were designed only for computer screens, and it was common for web pages to have a static design and a fixed size.

Then, when we started surfing the internet using tablets and mobile phones, fixed size web pages were too large to fit the viewport. To fix this, browsers on those devices scaled down the entire web page to fit the screen.

This was not perfect!! But a quick fix.

Setting The Viewport
HTML5 introduced a method to let web designers take control over the viewport, through the <meta> tag.

You should include the following <meta> viewport element in all your web pages:

<meta name="viewport" content="width=device-width, initial-scale=1.0">
This gives the browser instructions on how to control the page's dimensions and scaling.

The width=device-width part sets the width of the page to follow the screen-width of the device (which will vary depending on the device).

The initial-scale=1.0 part sets the initial zoom level when the page is first loaded by the browser.

Tip: If you are browsing this page with a phone or a tablet, you can click on the two links above to see the difference.

Size Content to The Viewport
Users are used to scroll websites vertically on both desktop and mobile devices - but not horizontally!

So, if the user is forced to scroll horizontally, or zoom out, to see the whole web page it results in a poor user experience.

Some additional rules to follow:

1. Do NOT use large fixed width elements - For example, if an image is displayed at a width wider than the viewport it can cause the viewport to scroll horizontally. Remember to adjust this content to fit within the width of the viewport.

2. Do NOT let the content rely on a particular viewport width to render well - Since screen dimensions and width in CSS pixels vary widely between devices, content should not rely on a particular viewport width to render well.

3. Use CSS media queries to apply different styling for small and large screens - Setting large absolute CSS widths for page elements will cause the element to be too wide for the viewport on a smaller device. Instead, consider using relative width values, such as width: 100%. Also, be careful of using large absolute positioning values. It may cause the element to fall outside the viewport on small devices.
