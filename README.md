# youtube-ai-summary-deploy-guide
Deploying YouTube video summary sites using Chapter 3.5, Vercel, and Render
## Preparation
- An account that can access the ChatGPT web version
- Vercel account https://vercel.com/
- Render account https://dashboard.render.com/
## Step 1
There are two ways to obtain YouTube subtitles:
  - Using third-party Python library yt-dlp https://github.com/yt-dlp/yt-dlp
  - Using the third-party library Puppeter of Nodejs, simulate opening a YouTube video page in a headless browser, and grab the timedtext interface
## Step 2
Build an API service using the open-source third-party OpenAI library in GitHub. Note that the third-party needs to support access token login.
Such As: https://github.com/zxxx98/go-chatgpt-api
## Step 3
Debug prompt to enable chatgpt to output a text in MDX format
## Step 4
Call GitHub's API and submit the generated MDX file to the web site repository (I am using the Vercel template here, which listens to repository changes and automatically initiates compilation)
## Step 5
~~Vercel compilation~~(Automatic Initiation)
## Done
-------------
#### Example URL: https://aivideosummary.top/
#### Vercel Recommended templates: https://vercel.com/new/templates/next.js/tailwind-css-starter-blog

Welcome everyone to join the discussion! 🌟 If there is anything you don't understand, please feel free to ask and we are happy to answer. 💡 Meanwhile, if you have any good ideas, please feel free to share them and let's explore and progress together! 🤝💭


