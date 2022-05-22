# Week 8 Lab Report
*Quincy Sewell, CSE 15L, Section A00*

## Markdown Parse Repository Links
The following is a link to my MarkdownParse repository:
[My MarkdownParse Repository](https://github.com/qsewell/markdownParseFinal)

It should be noted that the MarkdownParse file that I am using from that repository is called "MarkdownParse1.java", and *not* "MarkdownParse.java".

The following is a link to the MarkdownParse repository that I reviewed in Week 7's lab:
[Markdown Parse Repository That I Reviewed](https://github.com/aaronchan32/markdown-parser)

## Test 1
The following .md file represents the first test for both my own MarkdownParse implementation and the MarkdownParse implementation that I reviewed for Lab 7:

```
`[a link`](url.com)

[another link](`google.com)`

[`cod[e`](google.com)

[`code]`](ucsd.edu)
```

Based on the preview shown in VS Code, the expected output for such an input is:
```
[`google.com, google.com, ucsd.edu]
```

Here is my implementation of a JUnit test for this input:
![](JUnitTest1.jpg)

However, when run, my implementation of MarkdownParse gives the incorrect output, as can be seen from this terminal output of running the test:
![](Output1.jpg)

I do not think that there does exist a small code change (less than 10 lines) to my implementation of MarkdownParse that could make my program work for this input and related cases having to do with inline code and backticks, although there certainly could be one that I am overlooking. The reason why I think this would be a more involved change is because there are so many cases of backticks to consider (e.g., backticks within the square brackets, backticks where one is to the left of the opening square bracket and one is enclosed by the square brackets, backticks that enclose the square brackets, backticks where one is to the right of the closing square bracket and one is encolosed by the square brakcets, etc.). An implementation of a stack structure as a way of keeping track of pairs of backticks could be useful in correcting for these kinds of inputs.

