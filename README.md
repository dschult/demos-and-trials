README for webpage branch
=========================

This readme file appears in the gh-pages branch of the ideas repo.
It should who up at the bottom of the page when you first look at
the gh-pages branch. 

Looks like the files for the gh-pages branch are automatically used
for the associated webpage for the repo. That's pretty cool. To keep
them attached to the repo itself here's a method that I think describes
how NetworkX does it. 

  - Create a doc/ directory in your repo with the tools to build the 
    documentation webpages. 
  - In a local clone of the repo, clone the gh-pages branch into the
    doc/ directory.
  - create the html files for the docs you want on github.
  - copy them to the gh-pages directory (perhaps removing current 
    contents first)
  - do basically the following::
      cd gh-pages
      git add .
      git commit -m "Updating webpages with version x.xx.xx"
      git push origin gh-pages
  - the new pages should appear on http://**username**.github.io/**project**
