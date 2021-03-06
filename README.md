<img src="www/IDEA_logo_500.png"  height="120"/>

# MORTALITYMINDER

**NOTE:** For extensive details about [MORTALITYMINDER](https://mortalityminder.idea.rpi.edu/), please refer to the [MORTALITYMINDER WIKI](https://github.com/TheRensselaerIDEA/MortalityMinder/wiki).

The notes below are intended for users interested in cloning the repo and contributing code. 

## ABOUT MORTALITYMINDER
**MORTALITYMINDER** is a web application built on the [R Shiny](https://shiny.rstudio.com/) application framework, written primarily in R, with some UI functionality written in Javascript. It creates highly visual analysis of mortality data provided by [CDCWonder](https://wonder.cdc.gov/) and [County Health Rankings](http://www.countyhealthrankings.org/). You will find live versions of the app at the following locations:
* http://mortalityminder.idea.rpi.edu/ (primary)
* https://olyerickson.shinyapps.io/mortalityminder/ (secondary)
* Overview Video: http://bit.ly/mortalityminder_video_final

## LOCAL DEPLOYMENT
To run a local instance of MORTALITYMINDER, follow the steps below:

1. Clone the repository to your local setup; the directory `MortalityMinder` will be created.
2. Open RStudio and navigate to the `MortalityMinder` directory using the RStudio files tab.
3. Set the working directory to `MortalityMinder`
4. Double-click to open `app.R` and select `Run App` on the top-right corner of the code window.

## HOW TO CITE
If you use **MORTALITYMINDER** in your work, please use the following reference

Kristin P. Bennett and John S. Erickson, "MortalityMinder: an R-based, multi-view interactive presentation examining county-level factors associated with midlife mortality trends." [![DOI](https://zenodo.org/badge/197430685.svg)](https://zenodo.org/badge/latestdoi/197430685)

## DEVELOPMENT
The **MORTALITYMINDER** app is in active development and undergoes daily updates. Please be sure to consistently pull from master in your local setup. If you notice any bugs, create an issue. Please ensure issues have a descriptive title, and the comment should describe where the bug was found and how you were using the application. 

For all contributors, **any** changes made to the application should be written in a separate branch, and sent as a pull request. Please refrain from pushing changes directly to master, as we must ensure a working copy of the app at all times. When in doubt, follow this protocol:

1. Clone the repo...
2. cd into the resulting, new directory...
3. git checkout -b new_branch and git push origin (to claim their branch)
4. Code, code, code...
5. git commit -a -m "My awesome changes"
6. git commit -a -m "More awesome changes"
7. While still in your branch, do a git pull (only if others are also working on the branch)
8. Switch to master with git checkout master
9. Sync your master using git pull  <<< This is the important step!
10. Now switch back to your branch with git checkout new_branch
11. Now git commit -a -m "Final awesome changes" and git push origin
12. Now you can do a PR, which should be safe from conflict.

## ISSUES PROTOCOL
Found a bug? Please create an issue titled as a clear sentence describing the bug. In the description, please write as many details about your working environment as you can. Details include:
* Your machine and OS
* Your screen size and resolution
* The size of the **MortalityMinder** app window
* What **MortalityMinder** view did the bug appear on
* What state/and cause of death/and county, if applicable were selected when bug was found
* Any other information you may deem relevant to said bug

Would like to recommend an additional view or feature, or have a design recommendation? Create an issue and use the `enhancement` label. Your issue title should also indicate that it is a feature request on the title. Add as many details as you wish in the description section, the more you add, the more likely we will be able to bring this feature to life! You can also email feature requests to [erickj4@rpi.edu](mailto:erickj4@rpi.edu). Our team of open source developers will handle issues in a priority basis.
