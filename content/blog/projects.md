+++
title = "Project Based Learning"
date = 2025-07-23T10:48:49+09:00
draft = false
type = "blog"
featured = true
weight = 100  # Lower weight appears first in featured sections
description = ""
tags = ["pedagogy", "projects", "guide-to-success"]
topics = []
+++

# Projects in the Classroom

Computer Science is the perfect subject for practicing Inquiry and Project
based learning. In this article, I will explain why it is such a foundational
part of my pedagogy and provide a quick overview of how projects are structured
in my class to maximize student opportunities to learn how to learn.

## The Project-Based Subject

Project based learning is a perfect fit for Computer Science because of the
nature of the field. This is true for almost every subject which corresponds
directly to a real life profession. But this is particularly true for Computer
Science.

This is because Computer Programming, as a field, is project based. Real life
programming is a series of projects. Whether it is a simple project like a
homepage or a large project like Windows or MacOS, every website or application
ever created was created as a series of one or more projects.

### Assessment Code is Bad Code

In fact, the match between Computer Science and projects is so obvious that it
is difficult to come up with authentic assessments other than projects in a
programming class. On a traditional test, for example, students encounter
programming concepts in small example blocks of code, like the example below:

```javascript
for (let i = 0; i < 4; i++) {
  console.log(i);
}
```

This is a very bad example of a for loop if your goal is for students to be
able to use for loops in real life. First, this for loop is outside of a
function, but we rarely put any code outside functions in real programming
because enclosing them in functions makes it easier to develop and test the
code and allows easier code reuse. Second, the comparison condition for i is
hardcoded (`i<4`). While this is helpful for the very beginning of a student
learning to program, real programs almost never use a constant value here.
Instead, variable names are used. Finally, the contents of this loop merely
print to the screen. Once more, real programs rarely use for loops to loop a
single line of code unless that line of code is a function call to a function
the user had written. This might be a good test question to assess students
with a lower ability in programming.

The problem for testing is that it is difficult to legitimately assess a
student at a higher level of understanding of a for loop. Here is an attempt at
a code block which you could use for such a question:

```javascript
function mystery(x){
  return 3x+1;
}

function calculate(x) {
  let sum = 0;
  for (let i=0; i<x; i++){
    sum += mystery(i);
  }
  return x;
}

console.log(calculate(4))
```

Even this example is bad code - for example the function and variable names are
extremely unhelpful. But the things that make this bad code are necessary if
you are going to use it in a test question.

While there is sometimes value in showing students bad code, a test only
assesses their ability to read code, not write code. Worse, by only showing
them code which makes for good test questions, you are teaching them to write
confusing (or put another way, bad) code.

### Teaching Students to Write Good Code

Writing good code is much harder than reading bad code in much the same way
that writing a good paragraph is much harder than reading a bad one. So while
it is important that student learn to read bad code early in the process of
learning, having them write code becomes a better indicator of their ability
very quickly.

Every programming curriculum has students write code, but often the code
segments they are made to write are no longer than the code segments they are
made to read on a test.

For example, a lesson on for loops will often only require students read,
debug, or write 4-5 code segments, each containing only a single for loop. Very
few of these will contain more than 15-20 lines of code unless Java is the
programming language of instruction, and in that case the extra length is
solely because of the structure of the programming language.

By comparison, in a project I have written in Javascript (the language used in
all the examples here), I have a for loop with 13 lines of code in it, several
of which call other 10-20 line functions I had to write in that project. When
looking at real projects, most programmers would say that a small project runs
300-500 lines of code (depending upon the language). This is 20 times the
length of the assignments that most curricula have students spend 80% of their
time on.

In my experience, this massive gap in size means students feel uncomfortable
when working on a real project. Whether that project is a personal project or a
project for a course or company. This would be like students completing High
School without ever writing anything longer than a paragraph. You can certainly
learn a lot about writing by writing shorter segments, but if students are to
be expected to produce longer work, they must practice it.

## Real-life Projects

As I stated earlier, a small project runs 300-500 lines of code. This
encompasses almost all "hobbyist" projects that students might take on to add
to their resume. Real life programs can run into the millions of lines of code.

Even a project of 300 lines requires far more skill at managing complexity than
a project of 20 to 30 lines. Larger projects require the programmer to hold
more complexity in their heads while programming. Unless that programmer has
learned techniques to isolate the parts of the project from each other so they
can treat them as a number of isolate projects.

For many projects, the cycle will look something like this:

1. The programmer adds new features, code, or bugfixes to the project.
2. The project grows too large for the programmer to reason about.
3. The programmer redesigns some part of the project to reduce its complexity
   or isolate it from the rest of the project.
4. The programmer can now reason about the project enough to add more features,
   code, and bugfixes.

Step 3 - called "refactoring" by programmers - is the most challenging skill to
develop, and it can only really be practiced in projects large enough to need
them.

## How I Do Projects

When building a project for a programming class, I focus first on which skills
I want students to practice. For example, in the second unit of Web Design Foundations course, students need to incorporate style (colors, font sizes, etc) into their website via a programming language called CSS.

Now I start thinking about what project a student could create that would emphasize colors and other style elements. An important part of this is keeping in mind what skills the students do not yet have access to. In this class, multiple files are added in the third unit, which limits the sorts of projects students can do.

The project I've selected for this unit in previous years is an advertising website. Style and design are an important part of marketing and branding, which makes it a great project for this unit. In previous years, I have had them go back to the simple portfolio website they built in unit 1 and add style, but that has been moved to be part of the final project instead.

Knowing the skills and the project, I now start working on how I want to assess these skills. I will write more about this in another post. But having established this, it's now time to have the students start working.

Having set up the project, it's now time to have the students start working.

### The Project Learning Process

In my classes, we begin projects on the first day of the unit with a rubric review. Students begin working on their project regardless of the fact that they do not know the material in the unit yet.

I have found that students retain programming skills better when they discover the need for them. Starting the project from the beginning allows me to have conversations with students that tie the skills in the coursework directly to their projects. "Ah, you the color on this page to change as they scroll down? You need to look at the animations lesson."

Students split their time in class between the coursework and their projects, with the general idea being that they work on their project until they need to learn something new, at which point they go back to the coursework until they find what they need.

While obviously students aren't forced to follow this structure, and many students choose to basically follow a traditional system of doing all the coursework and then starting their project, students who do both need less reminding of concepts when they need to use them again in future projects.

Each week, students are required to complete a check-in following the Guide To Success (written about elsewhere). The only requirement in terms of progress is that they can increase their estimated score by at least 1 each week. This way, even students choosing to wait till the end are forced to do some of the planning and brainstorming before the very end of the project.

## Looking Ahead

This framework seems to me to be the most effective way to teach Computer Science. Because of its focus on projects to drive learning, it mimics the actual development project of most real-world programming projects.

In future articles in this series, I will look at the daily structure of project work in my classes and outline how I use a tool called the "Guide to Success" to promote student meta-thinking about their projects and learning.

