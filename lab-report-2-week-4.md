# Week 4 Lab Report
*Quincy Sewell, CSE 15L, Section A00.*

The following represents three changes made in a file called MarkdownParse.java, in an effort to address bugs in its code.

## Code Change 1
![](lab-report-2-codechangediff1.jpg)

Link to the test file for failure-inducing input that prompted the above change (note that the 5th empty line is not visible here, but is a part of the file):

[test-file-2.md](https://github.com/qsewell/markdown-parser/blob/main/test-file-2.md?plain=1)

The symptom initially caused by the above input was the following:

$ java MarkdownParse test-file-2.md  
Exception in thread "main" java.lang.OutOfMemoryError: Java heap space  
        at java.base/java.util.Arrays.copyOf(Arrays.java:3512)  
        at java.base/java.util.Arrays.copyOf(Arrays.java:3481)  
        at java.base/java.util.ArrayList.grow(ArrayList.java:237)  
        at java.base/java.util.ArrayList.grow(ArrayList.java:244)  
        at java.base/java.util.ArrayList.add(ArrayList.java:454)  
        at java.base/java.util.ArrayList.add(ArrayList.java:467)  
        at MarkdownParse.getLinks(MarkdownParse.java:19)  
        at MarkdownParse.main(MarkdownParse.java:30)

This can also be seen at the following link to the relevant commit for MarkdownParse.java:

[Commit1](https://github.com/qsewell/markdown-parser/commit/7f60c5a2c2935d5deef70ea59ecda40d8a803cda)

The bug 

## Code Change 2

## Code Change 3
