The file UNH_PhD_LaTeX includes several files that will help you create a fully-formatted UNH Grad School-approved PhD thesis.

*********************************************************
NOTE:
As of December, 2014, UNH moved thesis submission on-line. As a result, the committee signature page that is embedded within the actual body of the thesis will not contain any sigantures. Instead, the content in /unh_grad_print will be printed separately on any type of paper and turned into the graduate school.

To comply with these requirements and meet the submission deadline, I had to fudge the original thesis style sheet, "unh_thesis.sty", and create "unh_grad_req.sty". In them, you will find lots of 

\\ \hspace*{30 mm}
\hspace*{30 mm}
\hspace{30 mm}

in the "Define Committee Signauter Page" section. These set the horizontal offset of the names and affiliations. If you want more or less space, change "30 mm" to some other number of millimeters.

Happy writing,

Matthew Argall

*********************************************************

Below is an explanation of the folder's contents:

-- All of the "*.sty" files that you'll need to meet the required formatting

-- "Yourbib.bib" is the BibTeX file that will be used to make your bibliography. You'll need to populate this with your references or replace it with your own file.

-- "bookdefs_template.tex" is where you'll define all of the packages and commands you'll be using. You shouldn't need to change anything in here expect maybe to add directories to certain packages if their in other locations.

-- "Thesis-UNH.tex" is where all the magic happens. This is the file that's going to actually generate the document by calling all of the other files that you'll edit. There are comments in here about how to add chapters and all that. THIS IS THE FILE YOU'LL NEED TO TYPESET TO ACTUALLY GET AN OUTPUT. Remember, if you change the names of any of these other files or add new ones, you'll need to change or add the names in this file before you can typeset.

-- "frontmatter_template.tex" is where you'll put in the title, signature, and acknowledgment pages...basically everything that comes before the actual chapters themselves.

-- "/Chapters" contains ".tex" files for each chapter of the thesis. The files can be renamed, so long as the name is also updated in "Thesis-UNH.tex" is pretty much. If more chapters are needed, just add more files.

-- "/Appendices" contains ".tex" files for each appendix of the thesis. Add or remove files as needed, and make the necessary changes to "Thesis-UNH.tex"

-- "/unh_grad_print" contains the materials you must print and turn in to the graduate school. Copy and paste information from "Thesis-UNH.tex" into "unh_grad_print.tex", then typeset "unh_grad_print.tex".