<div align="center">

## DECLARING VARIABLES / CONSTANTS IN C


</div>

### Description

The tutorial is designed for the novice programmer

and the programmer who has never used structured

language before. It will give an impression how C

works. Experts skip this articles.
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Indee](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/indee.md)
**Level**          |Beginner
**User Rating**    |4.3 (65 globes from 15 users)
**Compatibility**  |C
**Category**       |[Miscellaneous](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/miscellaneous__3-1.md)
**World**          |[C / C\+\+](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/c-c.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/indee-declaring-variables-constants-in-c__3-824/archive/master.zip)





### Source Code

```
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.0 Transitional//EN">
<HTML><HEAD><TITLE>Tutorial-Declaring Variables/Constants in C</TITLE>
<META content="text/html; charset=windows-1252" http-equiv=Content-Type>
<META content="Inder Mohan Singh" name=Author>
<STYLE type=text/css>
<!--
 BODY{font-family: Arial; font-size:12pt;margin-left:1.5cm}
 TABLE{margin-left:1cm}
 P{margin-left:1cm; margin-right:1cm;}
 H1{color:#5f9ea0; font-size:20pt}
 H4{margin-left:1cm;color:#0000FF}
 B{background:#fffacd}
-->
</STYLE>
<META content="MSHTML 5.00.2614.3500" name=GENERATOR></HEAD>
<BODY>
<CENTER>
<H1><B>DECLARING VARIABLES / CONSTANTS IN C</B></H1></CENTER><BR>
<P>The tutorial is designed for the novice programmer and the programmer who has
never used structured language before. It will give an impression how C
works. <B>Experts skip this articles</B>.</P>
<P>
<H4>C is Case-Senstive</H4>
<P></P>
<P>If you are familiar with languages such as Pascal, one of the first diffrence
to notice in C is that it is case sensitive; uppercase and lowecase letters are
treated as separate characters. For example in C, the variable names
<B>length</B>, <B>Length </B>and <B>LENGTH</B> are three different variables. So
whenever entering the source code, be very careful to use the proper case.</P>
<P>Well I think the best way to learn is to write a simple C program and than I will
explain what all this jargon(source code) is about, so lets start by the following simple C program.</P>
<H4>A Simple Example of C Program</H4>
<TABLE border=0 cellPadding=0 cellSpacing=0 width="60%">
 <TBODY>
 <TR>
 <TD align=left bgColor=#f0f8ff><FONT color=#ff0000>
  <P>#include<stdio.h><BR><BR>/* Sample Program */<BR><BR>void main
  ()<BR>{<BR>     int age;<BR>    
  age = 31;<BR>     printf("My age is %d\n",
  age);<BR>}<BR><BR></P></FONT></TD></TR></FONT></TBODY></TABLE><BR>
<H4>Explanation</H4>
<P>Now lets take a closer look at each line in sample program. The first
line,<BR><BR>                <B>#include
<stdio.h></B><BR><BR>tells compiler to include the <I><B>stdio.h</B></I>
in the compilation. This file contains information needed by the program to
ensure the correct operation of standard library functions. In C there are
numbers of these types of files often referred to as <B><I>header files</I></B>.
Some programs will require more than one header file, so make sure that you
include these lines in your programs. <I>(I will discuss these files in details in
my future tutorials.)</I><BR>The second line,<BR><BR>       
        <B>/* Sample Program */</B> <BR><BR>is a
<B><I>comment</I></B>. In C, comments begin with the sequence /* and are
terminated by */. The C compiler ignores everything between these comment
symbols. This type of comment may extend over several lines. If the comment is
only one line long, then
use:<BR><BR>         <B>// Sample
Program </B><BR><BR>Did you noticed the blank lines following the comment line.
Well in C, blank lines are permitted and have no affect on the
program.<BR><BR>Ok now the
line,<BR><BR>         <B>void main()
</B><BR><BR>specifies the name of a <B><I>function</I></B>. All C programs begin
by calling the <B><I>main()</I></B> function.(I will discuss functions in
details in my future tutorials.)Void ststement indicates that the programs does
not return a value. <B>Void</B> means empty, or none.<BR><BR>The next line
consists of a single curly brace, <B>{</B>, that signifies the start of the
<B>main()</B> function.<BR><BR>Ok! guys lets get to the real thing, the first
line of code inside the <B>main()</B> function is <BR><BR>
         <B>int age;</B><br><br>
This line declares a variable called <B>age</B> and the <B>int</B> informs the compiler that it is
an integer. In C, <I>variables</I> must be declared before they are used. The declaration
process involves specifying the variable's name as well as its type. In this case, <B>age</B>
is of type <B>int</B>, which is C's <I>keyword</I> for integer. Integers are whole numbers.<br><br>
The next line is<br><br>
         <B>age = 31;</B><br><br>
which is assignment statement. It places the value 31 into the variable age. Notice
that C uses a single equal sign for assignment and also all the statements in C are
terminated by semicolon.<br><br>
The next line which ouputs information to the screen, is<br><br>
         <B>printf("My age is %d\n", age);</B><br><br>
Well this statement is very important for two reasons. First, it is an example of a
function call and secondly, it illustrates the use of C's standard output function,
<B>printf()</B>. There are two parts in this statement: the function name, which is <B>printf()</B>,
and its two arguments, <B>"My age is %d\n"</B> and<B> age</B>.(An <I>argument</I> is a value passed to the
function when it is called.)<br><br>
The first argument in the <B>printf()</B> function is a quoted string that may contain either
normal characters or <I>format codes</I> that begin with the percentage sign(%).A <I>format code </I>
informs <B>printf()</B> that a noncharacter item is to be displayed. In this case, the <B>%d</B> means
that an <I>integer</I> is to be output in decimal format. The value to be displayed is
found in the second argument, in this case <B>age</B>. The <B>\n</B> is a special code that tells
the printf() to issue a carriage-return-linefeed sequence, called a <I>new line</I> in C. This will
display <B>"My age is 31"</B>.To understand concept lets change the line to read:<br><br>
         <B>printf("%d is my age\n", age);</B><br><br>
The message now displayed is <B>"31 is my age"</B>. The point is that where the format command
occurs in the string determines where the second argument to <B>printf()</B> will be printed.
(Well printf() is substantially more powerful than illustrated by this example. I will
write tutorial on this in future.)<br><br>
OK at last the last line of the program is a closing curly braces,<B> }</B>, which tells the
compilers that this is the end of the <B>main()</B> function. The program execution is terminated.
<br><br>
Phew!! I think that's enough for todays lesson. Well I will be writing the next tutorial
about <B>C Data Types</B>.<br><br>
Bye! for now.
 </P></BODY></HTML>
```

