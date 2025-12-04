# StudentOpportunities
This repository hosts a GitHub page for students working with PIFSC and their mentors.  
If there's content you'd like to see added or changed, please [open an issue](https://github.com/noaa-pifsc/StudentOpportunities/issues)
or submit a pull request.  You can also reach out via [email](mailto:nmfs.pic.soc@noaa.gov).

---

## For Committee Members
The easiest way to update the [Student Opportunities GitHub Page](https://noaa-pifsc.github.io/StudentOpportunities/)
is with RStudio.  RStudio is approved NOAA/NMFS software that is both Windows-
and Mac-compatible.  

You will also need a PIFSC enterprise GitHub account.  [This site](https://sites.google.com/noaa.gov/nmfs-st-github-governance-team/faq)
(*internal to NOAA*) will help you get set up.  Once you have your account, you'll
need to connect your GitHub account with RStudio.  The same folks who get you
your account can help you with this.  

Once you've got RStudio on your computer and interacting with your enterprise 
GitHub account, you're ready to work with the GitHub Page.  Exciting!

The very first step is to give the committee chair your GitHub handle so that they
can invite you to collaborate in this repository (or repo).  You'll get an email
when they do that.  

Now, you need to connect your computer to this repo.  You
only need to do this once.  There are several ways to do this.  Here's one:  
Click the green "Code" button above: ![green code button](images/Code.png) and
copy the URL in the dialogue box that appears.  Now go to RStudio and select:
File > New Project > Version Control > Git  
Paste the URL as the Repository URL.  Name the project something that makes sense 
to you (perhaps, StudentOpportunities).  Put the project somewhere on your computer
that makes sense to you.  Best practice to is to click the box that says, "Open 
in a new session".  Click Create Project.  Voila!  Everything in this repository
is now on your computer and you're ready to get editing.

Edit the following files to edit the following aspects of the page:  
`index.Rmd` is the main landing page and "Upcoming events" tab in the header  
`cohorts.Rmd` is the "Cohorts" tab  
`resources.Rmd` is the "Resources" tab  
`highlights.Rmd` is the "Highlights" tab  

If you want to add additional tabs, you can create an RMarkdown file (.Rmd) for
them.  You'll also need to add the tab to the `_site.yml` file following the
convention of the other page elements.  

Once you've made edits to the Rmarkdown file(s), click the knit button at the top
of the editor in RStudio: ![blue ball of yarn with a knitting needle and the word knit](images/Knit.png)  
This will do three things:  
1. open a preview of the webpage you edited (handy for double-checking your edit 
before it goes live)   
2. create an updated version (or a new version if this the first time you've 
knit the file) of the synonymous HTML file in the `docs` folder of this repo  
3. update the `sitemap.xml` file in the `docs` folder.  
**You can edit and knit as much as you need without actually changing the GitHub Page.**

To update the GitHub Page you need to push your changes to GitHub.  This moves them
from your computer into the repository.  You can do it from RStudio.  In the 
Git pane you'll notice an M in a blue box next to the file(s) you updated: 
![white capital M in a blue box](images/M.png).  Click in empty box to its left. Click
"Commit" in the Git pane toolbar.  Type a brief message explaining your updated
in the box under "Commit message".  This could be something like, "added tour to
upcoming events".  Click commit below your message.  Close the dialogue box.  Click
"Pull".  This *pulls* any changes others have made in the repo onto your computer.  Close
the dialogue box.  Click "Push".  This *pushes* your change into the repo.  Close 
the dialogue boxes.

For small files, you can commit and push multiple files at once.  For larger files,
the enterprise GitHub gets cranky and then you have to troubleshoot things which
is annoying.  To avoid problems, commit and push the HTML file on its own.

Sometimes, when you push a few things in a row GitHub will email you that an action
was cancelled.  You can safely ignore this message.  

After you've pushed the final file, wait about 1 minute and then check the 
[Student Opportunities GitHub Page](https://noaa-pifsc.github.io/StudentOpportunities/) 
to see your change in place.

### Resources 
This site is built based on a [NMFS Open Science](https://nmfs-opensci.github.io/) [template](https://github.com/nmfs-opensci/NOAA-distill-website/tree/main).

This ReadMe is written in Markdown.  Checkout this [quick reference](https://www.markdownguide.org/cheat-sheet/) 
and the links therein to get started.  

The GitHub Page is written in RMarkdown, which is pretty similar to Markdown but
is specific to R.  [This reference](https://rstudio.github.io/cheatsheets/html/rmarkdown.html) 
will get you started.

[HappyGitWithR](https://happygitwithr.com/) is very handy when you need a reminder
of how to do something with GitHub and RStudio and when things go sideways.

---

### Disclaimer
This repository is a scientific product and is not official communication of the National Oceanic and Atmospheric Administration, or the United States Department of Commerce. All NOAA GitHub project code is provided on an ‘as is’ basis and the user assumes responsibility for its use. Any claims against the Department of Commerce or Department of Commerce bureaus stemming from the use of this GitHub project will be governed by all applicable Federal law. Any reference to specific commercial products, processes, or services by service mark, trademark, manufacturer, or otherwise, does not constitute or imply their endorsement, recommendation or favoring by the Department of Commerce. The Department of Commerce seal and logo, or the seal and logo of a DOC bureau, shall not be used in any manner to imply endorsement of any commercial product or activity by DOC or the United States Government.
