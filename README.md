# [Simulating Language](https://github.com/smkirby/simlang)

Copyright (c) 2009-2019 [**Simon Kirby**](http://www.lel.ed.ac.uk/~simon), with contributions from [Kenny Smith](http://www.lel.ed.ac.uk/~kenny/), [Jennifer Culbertson](https://jennifer-culbertson.github.io), [Andrew Smith](https://www.stir.ac.uk/people/256435)

This is a collection of interactive notebooks for a course taught in the [Centre for Language Evolution](http://lel.ed.ac.uk/cle) at Edinburgh showing how to model the evolution of language at all timescales - from individual utterances, through individual learning, cultural transmission, and biological evolution. This course covers many of the major research breakthroughs over the past two decades, and shows how easy it is to build simulations of language evolution. It is suitable for anyone, even without any background in coding, and uses only a very basic subset of the programming language, Python, throughout.

Although this course is taught in Edinburgh, you're welcome to try it at home if you're not a student using [Binder](https://mybinder.org/v2/gh/smkirby/simlang/master). I've also taught intensive versions of this course as week-long summer/winter schools, so please do get in touch if you're interested in this!

Please note that these documents are very much under construction and the text in particular is likely to be full of typos for some months yet!

## Course organisation, 2019

The course meets on Tuesdays, Thursdays, and Fridays throughout semester 2. When there is a lecture, the whole class meets together 14:00 - 15:00. When there is a lab, the class will split into three groups and meet either 14:00 - 15:00, 15:00 - 16:00, or 16:00 - 17:00. 

Students should read the lecture notes (by following the links above or below on the schedule, or on the notebook server for the course). These contain links to the papers we'll be reading as part of the course.

### Schedule (subject to change)

1. [Lecture: why simulate language? (15/01)](simlang_1_lecture.ipynb) ([slides](simlang_1_slides.pdf))
2. [Lab: python intro (17/01)](simlang_2+3_lab.ipynb) (plus [Introduction to notebooks](simlang_2_notebook_intro.ipynb))
3. Lab: python intro continued (18/01) (plus [Answers](simlang_2+3_answered.ipynb) and [Walkthrough](simlang_2+3_walkthrough.ipynb))
4. [Lecture: modelling innate signalling](simlang_4_lecture.ipynb) ([slides](simlang_4_slides.pdf)) (22/01)
5. [Lab: signalling (24/01)](simlang_5_lab.ipynb) (plus [Walkthrough](simlang_5_walkthrough.ipynb))
6. [Lecture: evolving signalling](simlang_6_lecture.ipynb) ([slides](simlang_6_slides.pdf)) (25/01)
7. [Lab: signalling in populations](simlang_7_lab.ipynb) (29/01)
8. [Lab: evolving signalling](simlang_8_lab.ipynb) (31/01)
9. [Lecture: evolving optimal signalling](simlang_9_lecture.ipynb) ([slides](simlang_9_slides.pdf)) (01/02)
10. [Lecture: from evolution to learning](simlang_10_lecture.ipynb) ([slides](simlang_10_slides.pdf)) (05/02)
11. [Lab: learned signalling](simlang_11_lab.ipynb) (07/02)
12. [Lecture: cultural evolution](simlang_12_lecture.ipynb) ([slides](simlang_12_slides.pdf)) (08/02)
13. [Lab: iterated learning](simlang_13_lab.ipynb) (12/02)

Break

14. Lecture: from individual to population ([slides](simlang_14_slides.pdf)) (26/02)
15. Lecture: Bayesian learning (28/02)
16. Lecture: iterated Bayesian learning (01/03)
17. Lab: iterated Bayesian learning (05/03)
18. Lecture: Greenbergian universals (07/03)
19. Lab: Greenbergian universals (08/03)
20. Lecture: compositionality (12/03)
21. Lab: compositionality from iterated learning (14/03)
22. Lecture: culture and innateness (15/03)
23. Lab: extending iterated Bayesian learning (19/03)
24. Lecture: evolution of learning bias (21/03)
25. Lecture: summary, and feedback on assignment 1 (22/03)

### Assessment

There are two assessments, in the form of two take-home exams with short-answer questions. Some questions will require running some simulations and presenting the results as a graph or set of graphs.

1. Assessment one, handed out Thursday 21st February, submission deadline Thursday 7th March noon (via Learn), marks returned Thursday 28th March.
2. Assessment two, handed out Thursday 28th March, submission deadline Thursday 11th April noon (via Learn), marks returned Thursday 2nd May.

For undergraduate students, the two assessments are weighted equally. For postgraduate students, the second assessment will count for 70% of the final mark.

## Using the interactive notebooks

The interactive Python notebooks work using a "Jupyter Server". The University of Edinburgh provides one that you can log into here: https://noteable.edina.ac.uk/login

Alternatively, if you're not a student at the University of Edinburgh, you can use Binder to interact with the notebooks on a temporary free server: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/smkirby/simlang/master)

If you're using the noteable service rather than Binder, you'll need to download the files onto the server. Once you've logged on to the noteable service you may have to either "reconnect" or "start" your server. Once you've done that you'll be given an interface that will let you upload notebooks and navigate the files you'll be creating. First, we need to upload the notebooks from this github site. To do that, you need to open a new notebook that you'll use to update the files regularly (whenever a new notebook is posted for example). Follow these steps:

- Click on the "new" menu.
- Select "Python 3". This will open a brand new notebook.
- In the first "cell" of the notebook, you need to enter some code that will handle the transfer from the github site. 

Copy and paste the following code into the cell:

	!rm -rf simlang
	!git clone https://github.com/smkirby/simlang
	!mkdir -p simlang_local
	!cp -nr simlang/* simlang_local


- Run this code by pressing SHIFT + ENTER. This will transfer all the current simlang content into your notebook server. It also makes a "local" copy of the code in a folder called "simlang_local". This is the one you should do your work in, safe in the knowledge any changed you make won't get overwritten.
- Rename your notebook something like "Update Course" by clicking on the "file" menu and then "rename"
- Save the notebook by clicking "file" and then "save and checkpoint".

Now you're done. You can close that browser tab. Next time you want to add new notebooks from the course website, just open the notebook "Update Course.ipynb" in the file list in the first noteable window and run that first cell again by pressing SHIFT + ENTER.

You can now click on the "simlang_local" folder in the file list in the noteable window and open any of the notebook files that are there. If you mess anything up, you can delete the notebook you're working on, run the update course notebook again and you'll have a fresh file to work from. (But be careful, you won't be able to undo this!)

[Simon Kirby](http://lel.ed.ac.uk/~simon/), University of Edinburgh, 2019

All aspects of this work aside from the Software itself is licensed under a [Creative Commons Attribution 4.0 International License](http://creativecommons.org/licenses/by/4.0/). For Software license, see [LICENSE file](LICENSE).
