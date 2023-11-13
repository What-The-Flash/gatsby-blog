# gatsby-blog
This repo has the steps required to create a quick and dirty Gatsby blog

## Following steps are what I think we need in Windows 

I don't normally do anything productive in Windows so I am happy to help, but you might need to do some searching for getting basics up and running in Windows as it will likely be quicker to find an answer than to wait for me to figure it out as I would be mostly guessing when it comes to that particualr OS. 

### Node Package Manager 

Get Node from here: [Node, Windows installer](https://nodejs.org/en/#home-downloadhead)

I don't know how to add commands to the Windows shell (will try to test this before suggesting to TechDave).

### VSCode

I use Visual Studio Code, but any IDE you are familiar with should be fine. [vsCode](https://code.visualstudio.com/download)

### Begin... 

- Create a folder somewhere
- Open a Command Prompt
- cd to the folder you have created for this blog
- type `npx gatsby new the-techdave-blog https://github.com/gatsbyjs/gatsby-starter-blog`

### npx should be doing something

So at this stage, `npx` should be pulling a copy of all the code your local javascript engine needs so that it can build the gatsby starter blog directly from github

At this stage, you don't need a a github or a hosting service or anything like that, we're just pulling everything we need so that we can start building something as a local test service. 

### starting that blog

from command prompt:

- cd into the new folder (my example is called `the-techdave-blog`)
- type `npm start`

### npm should be doing something

The Node Package Manager should now be building that started blog and eventually will probably open a web page for you. It should look something like the address; - `localhost:3000`

This should be an entirely working blog. Now finding your way around in Gatsby can take some effort, but basically you're going to be looking for something like so: 

- Open vscode
- You should see an option to `open a folder` - click it
- look for the folder you created at the start of this process
- vscode (or other) should now show you the full file structure on the left
- look inside the gatsby blog folder (\the-techdave-blog for eg)
- look inside src
- look inside pages
- look inside blog

Here you should see a bunch of .md files (I think that is the standard format) which are simple MarkDown files. These files are how you build your blog content. 

## The Blog is ready

Now of course there is customisation and all that good stuff, but basically this is now a finished product. You can run `npm build` but don't really need to, if you wanted to see it in the real world, open a Github account, get it uploaded to a repository, then open a netlify account (both free) and create a new site that is linked to your github repo, tell it how to build in the deploy setting and you will have a webpage that has a nonsense URL but is a perfectly working website, if you wanted to keep it, you just buy a domain name and point it at your netlify site. But for a budding developer the free URL from netlify is perfectly fine if you want to show a profile of your builds etc. 


