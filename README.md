# bethans-cookbook
The ultimate survival guide for cooking as a family (serves up to 8) and some secrets. Crafted with love by H&amp;M.

# Contributing guide
# Accessing the code
1. Clone the repo locally either through [GitKraken](https://support.gitkraken.com/working-with-repositories/open-clone-init/)
or just by running  
`git clone [url from the main repo page]`  
2. From [Overleaf](https://www.overleaf.com/8579461444jvqnhcqtbgfp).
Note: when working with Overleaf you MUST push your work back to GitHub when you are done. To do so, go  
`Menu -> GitHub -> Push changes from Overleaf to GitHub`  
and specify the commit message
Make sure you pull when opening after a while through similar steps.

# Making changes
The book is put together using the `xcookybooky` LaTeX package that ships installed by default.
The example subfolder contains some sample code that could compile immediately without errors.
You should be able to open that directory in TexLive or build manually with something like  
`pdflatex -interaction=nonstopmode -file-line-error book.tex`  

Please avoid commiting changed pdf files too often, only do that on more important commits.
This will keep the repository lightweight.

# Project structure
In a project folder (either `example` or `book`) there is a main tex file of the same name that contains all text which is not recipes, preamble and all the config.
Individual recipes are loaded from files in the `tex` directory. Follow the patterns there to create a new recipe. Not all fileds like oven temperature are required.
