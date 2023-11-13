# gatsby-blog
This repo has the steps required to create a quick and dirty Gatsby blog

## Following steps are what I think we need in Windows 

I don't normally do anything productive in Windows so I am happy to help, but you might need to do some searching for getting basics up and running in Windows as it will likely be quicker to find an answer than to wait for me to figure it out as I would be mostly guessing when it comes to that particualr OS. 

### Node Package Manager 

Get Node from here: [Node, Windows installer](https://nodejs.org/en/#home-downloadhead) - I downloaded the 20.9.0 LTS version.

I don't know how to add commands to the Windows shell (will try to test this before suggesting to TechDave). NB: I am using Windows 11 for this test.

- the windows installer is actually quite good here - it just offered to add to path as part of install
- I did tick the box on next screen to automatically install necessary tools
- A powershell window popped up to install a few extra modules, I just clicked ENTER to continue a few times

### VSCode

I use Visual Studio Code, but any IDE you are familiar with should be fine. [vsCode](https://code.visualstudio.com/download)
- 

### Begin... 

- Create a folder somewhere
- Open a Command Prompt
- check you have npm installed and working type: `npm -v` - if this runs without an error - it is working
- `cd` to the folder you have created for this blog
- type `npx gatsby new the-techdave-blog https://github.com/gatsbyjs/gatsby-starter-blog`

You will be asked to confirm installation of this package, after which the package will download and get things setup for you.

### npx should be doing something

So at this stage, `npx` should be pulling a copy of all the code your local javascript engine needs so that it can build the gatsby starter blog directly from github, this might be worth running twice, on the x220 and something newer to compare times, but, to be honest, once you have the blog downloaded and built, all page updates etc are really a light workload. 

You might see warnings during the download stage for gatsby, warnings are not show stoppers, ignore them.

For time, I wasn't tracking it as was doing this between other tasks, I would guess it took 5 minutes on my Windows PC, which is an AMD something from 2020 stuck on the back of a 100Mb internet connection that was also being used by several other devices in my household. Not a scientific measure of time, but it didn't feel too bad. 

### starting that blog

from command prompt:

- cd into the new folder (my example is called `the-techdave-blog`)
- type `npm start`

Previous step (npx gatsby new ...... ) was pulling all the packages it needed, this was probably more limited by internet speed etc. NPM Start is where we see the blog being built, this is where any local hardware weaknesses might show. This stage will be ineteresting to know any time differences between newer and older tech.

### npm should be doing something

The Node Package Manager should now be building that `getting started` blog and eventually will open a web page for you. It should look something like the address; - `http://localhost:8000`

This should be an entirely working blog. Now finding your way around in Gatsby can take some effort, but basically you're going to be looking for something like so: 

- Open vscode
- You should see an option to `open a folder` - click it
- look for the folder you created at the start of this process
- vscode (or other) should now show you the full file structure on the left
- look inside the gatsby blog folder (\the-techdave-blog for eg)
- look inside src
- look inside pages
- look inside blog

Here you should see a bunch of .md files (I think that is the standard format) which are simple MarkDown files. These files are how you build your blog content. Changes you make to the blog via vscode should be displayed each time you save the file, React should notice the new content and display it at next page reload. This part of the test should be quite quick (I think). Once the blog has been built and is running, changes to pages should not be a computer intensive activity (I think).

## The Blog is ready

Now of course there is customisation and all that good stuff, but basically this is now a finished product. You can run `npm build` but don't really need to, if you wanted to see it in the real world, open a Github account, get it uploaded to a repository, then open a netlify account (both free) and create a new site that is linked to your github repo, tell it how to build in the deploy setting and you will have a webpage that has a nonsense URL but is a perfectly working website, if you wanted to keep it, you just buy a domain name and point it at your netlify site. But for a budding developer the free URL from netlify is perfectly fine if you want to show a profile of your builds etc. 


