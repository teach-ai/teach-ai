---
permalink: /lectures/f16/week1.html
---

class: center, middle 

# EECS 398 :: 002, 003
## Computing for Computer Scientists

.copyright[
<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a>
** [Pat Pannuto](http://patpannuto.com) / Marcus Darden **
]

---

# What this class is about

---

# What this class is about

- This is not "Tools for Computer Scientists"

- Though, we will cover a lot of cool tools

- The goal is to give you the ability to pick up, learn, and use tools effectively

---

# This class is _NOT_ a set of tutorials

.left-column[
1. Log in to a CAEN machine in Linux
2. Press the "windows" key to open the application launcher and then type "gedit"
3. Now copy-paste the following block of code into the window:
    ```c
    #include <stdio.h>
    int main() { printf("Hello World\n"); return 0; }
    ```
4. Type "Ctrl-s" or click the "save" icon, save the file as "myprogram.c" in your home directory.
5. Press the "windows" key again and type "terminal"
6. In the window that appears, type "gcc myprogram.c -o myprogram"
7. Now type "./myprogram"
]
.right-column[
1. Open your favorite text editor and
write a basic "Hello World" program
2. Compile and run your program
]

---

# Lectures give you the "what" and the "why", homeworks are a self-guided tour on the "how"

- Lectures are designed to be interactive

- Lots of live coding, lots of mistakes!

- **Bring your laptop to every class**

---

# This is a very individual class

## Nothing in this class is hard...

--

## The second time you do it

![GPS Unit](img/gps.jpg)

---

# Collaboration

## Less than you're used to

- The goal is to build your _individual_ skills

- You will get the most benefit doing assignments on your own

## "The 15 Minute Rule"

- A little frustration is a good thing, a lot is a bad thing

   * Try to solve a problem on your own for 15 minutes before asking for help
   * After 15 minutes, ask for help!
   * Good rule of thumb outside of this class too

---

# Course Resources

## https://c4cs.github.io

- The course homepage. Everything is here or linked from here.

   * Homework assignments
   * Lecture materials
   * Syllabus, schedule, etc

- You can also get here from [canvas](https://umich.instructure.com/courses/106623/external_tools/3796)

### [Piazza](https://piazza.com/class/iqo81dkv68b1jb)

- Essentially high-latency digital office hours

   * All questions _private_ by default

### [Gradescope](https://gradescope.com/courses/3499/)

- Homework submission

   * Warning, their clocks are unsympathetic

- Entry code 9D87R9 <small>(also on course homepage)</small>

---

# Course Meeting Times and Locations

- **Section 002** 1670 BBB, Wednesday 1:30-3:00
- **Section 003** 1670 BBB, Friday 1:30-3:00

In general, you may attend any section, however if the classroom becomes
overfull, we will have to ask that you attend the section you are officially
registered for.

![Screenshot of Course Calendar](img/calendar.png)

<!-- Cute idea, but only works if this page is visible on load :(
<div id='calendar-loading'>Loading calendar...</div>
<div id='calendar'></div>
<a href="https://calendar.google.com/calendar/embed?src=4a0vvtkg11f6g0qs2er37gkkf8%40group.calendar.google.com&ctz=America/New_York" class="pull-right" target="_blank">Google Calendar link</a>
-->

---

# Work and Expectations

## This is a 1-credit course

- 1 credit = 4 hours of your life / week

   * 1.5 hours in lecture
   * 1.5 hours of homework
   * 3 times this semester: 2-3 hours of "advanced exercises"

## Grading

.column-33[
**40% Homework**

- One homework every week except the last week
- (Yes there is homework this week)
- Due at 10PM every Saturday
]

.column-33[
**30% Attendance & Participation**

- 12 weeks not counting the first week (or Thanksgiving)
- We'll take attendance every week, somehow
]

.column-33[
**30% Advanced Exercises**

- Explore a topic in more depth
- Two week window to turn them in
- _Must be turned in at office hours_
]

---

# You need will need your own computer for this class

### CAEN machines are **NOT** sufficient for this class

### If you don't have your own computer...

- Dog ate it
- TSA confiscated it on your flight to Michigan
- Drunk roommate confused it for a frisbee

The CSE department has some loaner laptops available for the semester<sup>&dagger;</sup>

- Contact Don Winsor: <a href="mailto:don@umich.edu">don@umich.edu</a>

.footnote[
<sup>&dagger;</sup>For people with genuine need, please don't abuse this
]

---

# Course staff

<!-- again, cute idea, again only works if visible on load :(
<iframe width="100%" height="350px" src="/#syllabus"></iframe>
-->

![Screenshot of Course Staff](img/course_staff.png)

### ^another screenshot of [c4cs.github.io](https://c4cs.github.io/#staff)

[c4cs]: https://c4cs.github.io


---

<div style="display: flex;">
<div style="margin: auto;">
.center-center[
# `</administrivia>`
]
</div>
</div>

---

class: full-dark-image
background-image: linear-gradient(rgba(255,255,255,0.9),rgba(255,255,255,0.9)), url(img/take_a_break.jpg)

# Take A Break

### &nbsp;

.left-column[
1. Take a selfie
2. E-mail [c4cs-photos@umich.edu](mailto:c4cs-photos@umich.edu) with...
   - Your name
   - Your picture
   - One thing you want to get out of this course
   - Anything else you want us to know about you
      - Preferred nickname
      - Special considerations
      - Awesome trivia
3. Meet a stranger
   - Preferably not the person right or left, maybe turn around behind you?
]
.right-column[
.padding-lr-40[
![Selfie of Pat from this morning](img/selfie.jpg)
]
]

.footnote[
.opacity-25[
<small><em>Photo credit https://feministspectator.princeton.edu/2016/02/24/hamilton/</em></small>
]
]


---

<div style="display: flex;">
<div style="margin: auto;">
.center-center[
# `<class>`
]
</div>
</div>

---

# Straw Poll: Who has Linux on their laptop?

--

## Having something Unix-like on your machine will make your CS life at Michigan much more pleasant

- This not because Unix is "better"
- This does not mean you cannot use Windows

--

## Come October-ish this is going to be a lot easier

- OS X has it built in
- [Linux subsystem for Windows](https://msdn.microsoft.com/en-us/commandline/wsl/faq) in the "Windows 10 Anniversary Update"

---

# What is a computer, really?

--

## What is a "Virtual Machine"

#### How might we make one?

--

# &nbsp;

### VMs are a safe playground for you to explore

### And a common platform for teaching

# &nbsp;

--

## For Homework 1, you'll install a VM to use this term

---

# Live exercises in a Unix environment

- What's a shell?

- Why learn this stuff in 2016?

- The critical basics:

   - Where am I?

   - What's nearby?

- What commands have you seen before?

--

.left-column[
- cat
- cd
- chmod/chown/chgrp
- clear
- cp
- diff
- echo
- fg/bg/jobs [ctrl-z]
- grep
- help
- kill
]
.right-column[
- ls
- man
- mkdir
- mv
- pwd
- rm
- sleep
- tail
- touch
- true
- whoami
]

---

class: center, middle

# Welcome to C4CS
## Looking forward to a great semester!
