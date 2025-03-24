# Processing_code folder

This folder contains code for processing data.

It's the same code done 3 times:

* First, an R script that does all the cleaning.
* Second, a Quarto file which contains exactly the same code as the R script but produces an .html report.
* Third, my current favorite, is a Quarto file with an approach where the code is pulled in from the R script and run, and an .html report produced.

The last version has the advantage of having code in one place for easy maintenance (writing/debugging), and reusing by pulling the code chunk into the Quarto file for a nice combination of text/commentary and code.
