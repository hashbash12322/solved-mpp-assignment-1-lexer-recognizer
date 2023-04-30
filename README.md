Download Link: https://assignmentchef.com/product/solved-mpp-assignment-1-lexer-recognizer
<br>












Contents

1 Specification                                                                                             2

1.1 Phase 1: Lexer  …………………………………………………………………….. 3

1.2 Phase 2: Recognizer  ………………………………………………………………. 3

2 Requirements                                                                                            3

3 Change Log                                                                                              4




Assignment 1version 1.1

After completing this assignment, you will be able to

<ul>

 <li>define formally lexicon of a programming language.</li>

 <li>use ANTLR to implement a lexer for a programming language.</li>

 <li>define formally grammar of a programming language.</li>

 <li>use ANTLR to implement a recognizer for a programming language.</li>

</ul>

1 Specification

In this assignment, you are required to write a lexer and a recognizer for a program written in MC. To prepare for this assignment, you need to:

<ul>

 <li>Download initial.zip and unzip it.</li>

 <li>Download antlr-4.7.1-complete.jar from <a href="http://antlr.org">org</a>, set the environment variable ANTLR_LIB to this file and follow the íntructions in initial/README.txt to test the initial code.</li>

 <li>Remove all files in folders initial/src/main/mp/utils, initial/src/main/mp/astgen, ini­tial/src/main/mp/checker, initial/src/main/mp/codegen.</li>

 <li>Delete files initial/src/test/<a href="http://ASTGenSuite.py">py</a>, initial/src/test/<a href="http://CheckerSuite.py">CheckerSuite.py</a>, and ini­tial/src/test/<a href="http://CodeGenSuite.py">CodeGenSuite.py</a></li>

 <li>Comment out five lines 11-15 and from line 103-end of file initial/src/test/<a href="http://TestUtils.py">py</a> and test the initial code again with just three following íntructions:</li>

</ul>

python <a href="http://run.py">run.py</a> gen

python <a href="http://run.py">run.py</a> test LexerSuite

python <a href="http://run.py">run.py</a> test ParserSuite

<ul>

 <li>Change folder initial into assignment1 To complete this assignment, you need to:</li>

 <li>read carefully the specification of MP language</li>

 <li>Modify MP.g4. in the initial code to describe formally MP language.Please fill in your id in the header of this file.</li>

</ul>




<ul>

 <li>Add more test in LexerSuite and ParserSuite in the initial code.</li>

</ul>

This assignment is divided two phases: lexer phase and recognizer phase. These phases are assessed independently.

1.1 Phase 1: Lexer

In this phase, you are required to write a lexer for a program written in ANTLR. To complete this phase, you need to:

<ul>

 <li>Modify MP.g4 to detect tokens in MP language.</li>

 <li>Make 100 testcases for LexerSuite to test your code.</li>

 <li>For lexical errors, please print out as follows:</li>

</ul>

– “ErrorToken “+ &lt;char&gt;: when the lexer detects an unrecognized character

– “Unclosed string: “+&lt;unclosed string&gt;: when the lexer detects an unterminated string.

– “Illegal escape in string: “+&lt;wrong string&gt;: when the lexer detects an illegal escape in string. The wrong string is from the beginning of the string to the illegal escape.

<ul>

 <li>You can assume that there is only one error in each test case. 2 Phase 2: Recognizer</li>

</ul>

In this phase, you are required to write a recognizer for a program written in MP. To complete this phase, you need to:

<ul>

 <li>Modify MP.g4.</li>

 <li>Make 100 testcases for ParserSuite to test your code.</li>

 <li>You can assume that there is at most one error in each test case.</li>

</ul>

2 Requirements

Note that you must NOT compress your files when submit them. You may test your code at the website:

<a href="http://www.cse.hcmut.edu.vn/onlinejudge,">http://www.cse.hcmut.edu.vn/onlinejudge,</a> but you MUST submit three files MP.g4, <a href="http://Lex-erSuite.py">Lex­</a><u>erSuite.py</u> and <a href="http://ParserSuite.py">ParserSuite.py</a> in BKeL.

The deadline of both phases of assignment 1 is announced in the class website.

You must complete the assignment by yourself and do not let your work seen by someone else, otherwise, you will be punished by the university rule for plagiarism.




3 Change Log

From 1.0,

. Add the preparation instructions for the assignment 1.