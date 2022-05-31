# Week 10 Lab Report
*Quincy Sewell, CSE 15L, Section A00*

This is my fifth and final lab report for CSE 15L, Section A00 during Spring Quarter 2022 at UCSD. It focuses on two particular .md test files which induced different 
outputs for my implementation of MarkdownParse and the implementation of MarkdownParse provided to me in Week 9 of this course.

## How I Located Tests with Different Results
In order to find these two .md test files amid the 652 total .md test files in the test-files/ directory, I began by running the following bash script in each of the repositories containing the implementations of MarkdownParse using `bash script.sh > results.txt` (where script.sh was the name of the file containing the following bash script):

![](lab-report-5-bash-script.jpg)

In other words, for each file in the test-files/ directory, I printed out the name of the file followed by its corresponding output when MarkdownParse was run on it, and I did this for each of the two implementations of MarkdownParse. I also appended all of this output to to a text file named results.txt in each repository (this corresponds to the `> results.txt` part of the command mentioned earlier, and I later renamed the text file in _my_ repository results2.txt so that I could further distinguish between the two).

Next, in my own repository, I used `vimdiff results2.txt ../cse15lsp22-markdown-parser/results.txt` to compare the two text files alongside each other in vim. The following image presents a portion of the resulting display:

![]()
