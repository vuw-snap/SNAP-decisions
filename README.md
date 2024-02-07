the main depository for the VUW-SNAP website.<br>

we use Quarto to create the website documents <br>
https://quarto.org/docs/get-started/hello/text-editor.html <br>
https://quarto.org/docs/guide/ <br>
the quarto documents are in the other depository "snap-web" <br>

basic structure is <br>
_quarto.yml : sets out framework of website <br>
various xxx.qmd files contain markdown versions of the final .html files <br>
styles.css where you control some of formatting in the form of  <br>
the index.qmd file will be the opening page <br>

basic instructions: <br>
clone SNAP-web  <br>
I put my files into a local directory called SNAP-decisions-testing <br>
alter the files with your editor <br>
from outside of your directory type  <br>
     quarto preview mysite (mysite=SNAP-decisions-testing) <br>
this will generate the html <br>
the html will be in directory "_site" unless you point to another directory in _quarto.yml  <br>
for example I put my changes into a directory called SNAP-decisions by adding the following line in _quarto.yml <br>
output-dir: /Users/tricia/Documents/GitHub/SNAP-decisions <br>
then from inside SNAP-decisions (NOT SNAP-decisions-testing) do the standard git styff <br>
git init <br>
git status <br>
git add --all <br>
git commit -m "add multiple files" <br>
git push https://github.com/vuw-snap/SNAP-decisions.git main <br>
