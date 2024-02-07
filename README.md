the main depository for the VUW-SNAP website.


we use Quarto to create the website documents
https://quarto.org/docs/get-started/hello/text-editor.html
https://quarto.org/docs/guide/
the quarto documents are in the other depository

basic structure is
_quarto.yml : sets out framework of website
various xxx.qmd files contain markdown versions of the final .html files
styles.css where you control some of formatting in the form of 
the index.qmd file will be the opening page

basic instructions:
clone SNAP-decisions 
I put my files into a directory called SNAP-decisions-testing
alter the files with your editor
from outside of your directory type 
     quarto preview mysite (mysite=SNAP-decisions-testing)
this will generate the html
the html will be in directory "_site" unless you point to another directory in _quarto.yml 
for example I put my changes into a directory called SNAP-decisions by adding the following line in _quarto.yml
output-dir: /Users/tricia/Documents/GitHub/SNAP-decisions
then from inside SNAP-decisions (NOT SNAP-decisions-testing) do the standard git styff
git init
git checkout -b SNAP-decisions-1
git status
git add --all
git commit -m "add multiple files"
????
git status (check what branch are you on)
git push https://github.com/vuw-snap/SNAP-decisions.git main
