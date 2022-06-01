# Week 10 Lab Report
*Quincy Sewell, CSE 15L, Section A00*

This is my fifth and final lab report for CSE 15L, Section A00 during Spring Quarter 2022 at UCSD. It focuses on two particular .md test files which induced different 
outputs for my implementation of MarkdownParse and the implementation of MarkdownParse provided to me in Week 9 of this course.

## How I Located Tests with Different Results
In order to find these two .md test files amid the 652 total .md test files in the test-files/ directory, I began by running the following bash script in each of the repositories containing the implementations of MarkdownParse using `bash script.sh > results.txt` (where script.sh was the name of the file containing the following bash script):

![](lab-report-5-bash-script.jpg)

In other words, for each file in the test-files/ directory, I printed out the name of the file followed by its corresponding output when MarkdownParse was run on it, and I did this for each of the two implementations of MarkdownParse. I also appended all of this output to to a text file named results.txt in each repository (this corresponds to the `> results.txt` part of the command mentioned earlier, and I later renamed the text file in _my_ repository results2.txt so that I could further distinguish between the two).

Next, in my own repository, I used `vimdiff results2.txt ../cse15lsp22-markdown-parser/results.txt` to compare the two text files alongside each other in vim. The following image presents a portion of the resulting display (left is my implementation's results, right is the results of the implementation I was given in Week 9):

![](lab-report-5-vimdiff.jpg)

From this, it is clear that many tests have the same output for both implementations of MarkdownParse, which is reassuring, but the tests 22.md and 32.md are two tests that have different output depending on which implementation of MarkdownParse one uses - they are highlighted horizontally with purple bars. This is how I located these two tests.

## Links to Test Files With Different Results
The following is a link to the test file 22.md, out of which different results were produced depending on the MarkdownParse implementation:
[22.md](https://github.com/nidhidhamnani/markdown-parser/blob/main/test-files/22.md?plain=1)

And this is a link to the test file 32.md (it likewise had different results):
[32.md](https://github.com/nidhidhamnani/markdown-parser/blob/main/test-files/32.md?plain=1)

## Examination of Different Outputs for 22.md
For the test file 22.md, neither implementation of MarkdownParse gave the correct output; as can be verified by using the preview of a Markdown file's rendering in Virtual Studio Code, the correct (expected) output should be:

[ti\*tle]

My implementation of MarkdownParse gave the following output (this can also be seen from the result of the `vimdiff` command discussed and displayed earlier):

![](lab-report-5-22-output2.jpg)

The implementation of MarkdownParse I was given in Week 9 gave the following output (this can also be seen above):

![](lab-report-5-22-output1.jpg)

## Examination of Different Outputs for 32.md
