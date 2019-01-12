# [Simulating Language](https://github.com/smkirby/simlang)

[**Simon Kirby**](http://www.lel.ed.ac.uk/~simon) January 2019


This is a collection of interactive notebooks for a course taught in the Centre for Language Evolution at Edinburgh showing how to model the evolution of language at all timescales - from individual utterances, through individual learning, cultural transmission, and biological evolution. This course covers many of the major research breakthroughs over the past two decades, and shows how easy it is to build simulations of language evolution. It is suitable for anyone, even without any background in coding, and uses only a very basic subset of the programming language, Python, throughout.

## Course organisation, 2019

**First class: Tuesday 22nd January, 14:10 - 15:00, Gaddum Lecture Theatre, 1 George Square**

The course meets on Tuesdays, Thursdays, and Fridays throughout semester 2. When there is a lecture, the whole class meets together 14:00 - 15:00. When there is a lab, the class will split into three groups and meet either 14:00 - 15:00, 15:00 - 16:00, or 16:00 - 17:00. Assignments of students to groups will be carried out after the first lecture using an online sign up system.

### Schedule (subject to change)

1. [Lecture: why simulate language? (15/01)](simlang_1_lecture.ipynb) ([slides](simlang_1_slides.pdf))
2. [Lab: python intro (17/01)](simlang_2+3_lab.ipynb) (plus [Introduction to notebooks](simlang_notebook_intro.ipynb))
3. Lab: python intro continued (18/01) [Answers](simlang_2+3_answered.ipynb), [Walkthrough](simlang_2+3_walkthrough.ipynb)
4. Lecture: modelling innate signalling (22/01)
5. Lab: signalling (24/01)
6. Lecture: evolving signalling (25/01)
7. Lab: signalling in populations (29/01)
8. Lab: evolving signalling (31/01)
9. Lecture: evolving optimal signalling (01/02)
10. Lecture: from evolution to learning (05/02)
11. Lab: learned signalling (07/02)
12. Lecture: cultural evolution (08/02)
13. Lab: iterated learning (12/02)

Break

14. Lecture: from individual to population (26/02)
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

1. Assessment one, handed out Wednesday 27th February, submission deadline Thursday 7th March noon (via Learn), marks returned Thursday 28th March.
2. Assessment two, handed out Thursday 28th March, submission deadline Thursday 25th April noon (via Learn), marks returned Thursday 16th May.

For undergraduate students, the two assessments are weighted equally. For postgraduate students, the second assessment will count for 70% of the final mark.

## Using the interactive notebooks

The interactive Python notebooks work using a "Jupyter Server". The University of Edinburgh provides one that you can log into here: https://noteable.edina.ac.uk/login

We will talk you through how to use the notebooks in the lab, but I'll outline the steps here too. After you've logged on to the noteable service you may have to either "reconnect" or "start" your server. Once you've done that you'll be given an interface that will let you upload notebooks and navigate the files you'll be creating. First, we need to upload the notebooks from this github site. To do that, you need to open a new notebook that you'll use to update the files regularly (whenever a new notebook is posted for example). Follow these steps:

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

This work is licensed under a [Creative Commons Attribution 4.0 International License](http://creativecommons.org/licenses/by/4.0/)
