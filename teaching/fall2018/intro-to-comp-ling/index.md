---
layout: page
title: Introduction to Computational Linguistics
tagline: University of Rochester (Spring 2018)
---

# Description

This course covers foundational concepts in computational linguistics
and is designed for students with a strong background in formal
linguistic methods but little or no programming experience. Topics
include introductory formal language theory and probability theory,
finite state phonological and morphological analysis, generative and
discriminative approaches to shallow syntactic parsing (e.g.
part-of-speech tagging, chunking) and shallow semantic parsing (e.g.
semantic role labeling), and bottom-up and top-down algorithms for
syntactic and semantic parsing. Major focus is placed on deploying
techniques used in computational linguistics to advance linguistic
theory and developing students' ability to implement these techniques.

# Logistics

| **Classroom**    | 513 Lattimore Hall                                      |
| **Time**         | Monday & Wednesday 10:25-11:40am                        |

| **Instructor**   | [Aaron Steven White](http://aswhite.net)                |
| **Office**       | 511A Lattimore Hall                                     |
| **Office hours** | Tuesday 9:30-10:30am & 12:30-1:30pm (or by appointment) |
| **Email**        | aaron.white@rochester.edu                               |

| **TA**           | Venkat Govindarajan                                     |
| **Office**       | 4107 Wegmans Hall                                       |
| **Email**        | vgovinda@ur.rochester.edu                               |

# Readings

There will be a substantial amount of reading per week. A tentative
schedule is provided below. This tentative schedule will almost
certainly change as the semester goes forward. Consult the table below for
the most current list.

# Homework

Homeworks will be assigned weekly or biweekly throughout the semester, except
during the first three weeks, during which there will be a short programming
homework due every class. Most homeworks after the first three weeks of the
course will involve both a programming component and a written component, though
the relative balance between the two will vary. A template to guide you through
both components will be provided through [Overleaf](http://overleaf.com).

All written work *must* be produced in LaTeX (using the provided
template), and it must be submitted through
[Overleaf](http://overleaf.com) (where templates will be hosted). Do not
hand in handwritten work or email me electronic documents. You will not
receive credit for that assignment unless you subsequently turn the
assignment in through [Overleaf](http://overleaf.com) (subject to late
penalties).

All coding work must be done in Python, and like written work, it must also be
submitted through Overleaf. You can upload coding assignments to Overleaf by
right- or CTRL-clicking on a directory in the project sidebar and clicking
Upload from Computer. Do not submit coding work by email.

# Midterm

There will be a take-home midterm, which will tentatively be made available on
Wednesday, Oct. 10 and will be due two weeks later (Wednesday, Oct. 24).

# Final

For *LIN224 students*, there will be a take-home final exam, which will be made
available on Wednesday, Dec. 7 and will be due one week later (Wednesday, Dec.
14).

For *LIN424 students*, there will be a final paper, which will be due on
Wednesday, Dec. 14. A 500-word prospectus for this paper will be due Monday,
Nov. 12. More information will be made available closer to that date.

LIN224 students may opt to write a final paper in place of the final
exam, but they should do so with the knowledge that this paper will be
graded relative to a rubric designed for graduate student papers.

# Tools

One major aim of this class is to familiarize you with the computational
linguist's tools of the trade. The two we will be working with are
LaTeX, for all written work, and Python, for programming assignments.

You will be expected to learn LaTeX on your own. There are plenty of
tutorials online for doing this, including a few targeted specifically
at linguists. Please do not ask me if you can use a word processor
instead. The answer will be no.

You will **not** be expected to learn Python on your own; we will spend the
first two full weeks of class working through a Python tutorial. But
because there is a lot of content to cover in this course, this section
of the course will be relatively brief and fast-paced. If it turns out
that you need extra help on some basic programming concept, it is your
responsibility to seek out help as soon as that becomes clear to you.
This is especially important because programming assignments will build
in complexity, and so if you get stuck early, you have trouble
throughout the rest of the course. Please do not wait to get help.

*Note for Windows 10 users:* Some Python packages that we will use have known
issues on Windows. As such, you must install either the [Ubuntu Linux
subsystem](https://docs.microsoft.com/en-us/windows/wsl/install-win10) or
[Docker](https://docs.docker.com/docker-for-windows/) and then install Python
within the virtual machine you chose. This will require you to gain a basic
competence in using the command line. You are responsible for building this
competence if you do not already possess it. Please do not try to use a
Windows-based Python installation. You will have issues.

# Final grades

The grading breakdown is: (bi)weekly assignments (50%), midterm (15%),
final (25%), participation (10%). (Percentages represent percent of
total grade.)

# Late work

Assignments should be submitted by 11:59pm the day they are due. An automatic
10% deduction will be applied after this time, and you must explicitly notify
both Venkat and me by email when you turn the late assignment in or you will not
receive any credit.

Starting from the end of class, assignments will lose 10% per day late according
to the UTC time-stamp of submission that Overleaf reports. Late assignments may
not be turned in for credit after a week unless explicit permission was sought
before the due date.

# Exceptions

Students will not be penalized because of important civic, ethnic,
family or religious obligations, or university service. You will be have
a chance, whenever feasible, to make up within a reasonable time any
assignment that is missed for these reasons. Absences for these reasons
will count as excused for the sake of the participation grade. But it is
your job to inform me of any expected absences in advance, as soon as
possible.

# Honesty

All assignments and activities associated with this course must be
performed in accordance with the University of Rochester's Academic
Honesty Policy. More information is available at:
<http://www.rochester.edu/college/honesty/>.

# Personal needs

Any student who needs special accommodations due to a disability should
let me know privately, at the start of the semester.

# Schedule

Aug. | 29 | Introduction to Computational Linguistics | -                                        | -    |
Sept. | 05 | First steps in Python                    | Downey 2015, Ch. 1-4                     | HW0  |
Sept. | 10 | Control flow in Python                   | Downey 2015, Ch. 5-9                     | HW1  |
Sept. | 12 | Collections in Python                    | Downey 2015, Ch. 10-12, 14               | HW2  |
Sept. | 17 | Classes in Python                        | Downey 2015, Ch. 15-18                   | HW3  |
Sept. | 19 | Working with text in Python              | Jurafsky & Martin 2018, Ch. 2            | -    |
Sept. | 24 | Finite state automata                    | Sipser 2013, Ch. 1                       | HW4  |
Sept. | 26 | Finite state transducers                 | Jurafsky & Martin 2009, Ch. 3            | -    |
Oct. | 01 | Context free grammars                     | Sipser 2013, Ch. 2.1-2.3                 | HW5  |
Oct. | 03 | The CKY algorithm                         | Jurafsky & Martin 2009, Ch. 13.1-13.4.1  | -    |
Oct. | 08 | The Earley algorithm                      | Jurafsky & Martin 2009, Ch. 13.4.2       | -    |
Oct. | 10 | Shift-reduce parsing                      | Jurafsky & Martin 2018, Ch. 14.1-14.4    | HW6  |
Oct. | 17 | Mildly context sensitive formalisms       | Clark 2014                               | -    |
Oct. | 22 | Parsing MCFG/LCFRS                        | Kallmeyer 2013                           | -    |
Oct. | 24 | Basic probability theory I                | Goldwater 2016, Sec. 1-4                 | MT   |
Oct. | 29 | Basic probability theory II               | Goldwater 2016, Sec. 5                   | -    |
Oct. | 31 | \textit{N}-gram models                    | Jurafsky & Martin 2018, Ch. 4            | -    |
Nov. | 05 | Basic information theory                  | Manning & Schütze 1999 Ch. 2.2           | -    |
Nov. | 07 | Collocation measures                      | Manning & Schütze 1999 Ch. 5             | HW7  |
Nov. | 12 | Na\"ive Bayes                             | Jurafsky & Martin 2018, Ch. 6            | (P)  |
Nov. | 14 | Probabilistic Topic Models                | Steyvers & Griffiths 2007                | HW8  |
Nov. | 19 | Hidden Markov Models                      | Jurafsky & Martin 2018, Ch. 9.1-9.4      | -    |
Nov. | 21 | The Forward-Backward algorithm I          | Jurafsky & Martin 2018, Ch. 9.5          | -    |
Nov. | 26 | The Forward-Backward algorithm II         | -                                        | -    |
Nov. | 28 | Probabilistic context free grammars       | Jurafsky & Martin 2018, Ch. 13.1-13.7    | -    |
Dec. | 03 | The Inside-Outside algorithm I            | Manning & Schütze 1999, Ch. 11           | HW9  |
Dec. | 05 | The Inside-Outside algorithm II           | -                                        | -    |
Dec. | 07 | Review I                                  | -                                        | HW10 |
Dec. | 12 | Review II                                 | -                                        | -    |


# References

* Clark, A. 2014. [An introduction to multiple context free grammars for linguists]. ms.
* Downey, A.B. 2015. [*Think Python: How to Think Like a Computer Scientist*] 2nd ed. Green Tea Press.
* Heinz, J. 2011. [Computational Phonology -- Part I: Foundations]. *Language and Linguistics Compass*. Blackwell.
* Manning, C. & H. Schutze. 1999. [Foundations of Statistical Natural Language Processing]. MIT Press.
* Joshi, A.K., and Y. Schabes. [Tree-adjoining grammars]. *Handbook of Formal Languages* 3: 69-124.
* Jurafsky, D., & Martin, J. H. 2009. [*Speech and Language Processing*] 2nd ed. Pearson.
* Jurafsky, D., & J.H. Martin. 2018. [*Speech and Language Processing*][1] 3rd ed.
* Kaplan, R. & M. Kay. 1994. [Regular models of phonological rule systems] *Computational Linguistics* 20:3. 331–378  
* Sipser, M. 2013. [*Introduction to the Theory of Computation*]. 3rd ed. CENGAGE Learning.
* Sutton, C. & A. McCallum 2011. [An Introduction to Conditional Random Fields]. *Foundations and Trends in Machine Learning* 4:4. 267–373.
* Stabler, E. 2010. [Computational perspectives on minimalism]. In C. Boeckx, ed. *Oxford Handbook of Linguistic Minimalism*. 616-641. Oxford University Press.
* Steedman, M. & J. Baldridge. 2011. [Combinatory Categorial Grammar]. In R. D. Borsley and K. Börjars (eds), *Non-Transformational Syntax: Formal and Explicit Models of Grammar*. Wiley-Blackwell, Oxford, UK.
* Steyvers, M. & T. Griffiths. 2007. [Probabilistic Topic Models]. In T. Landauer, D. McNamara, S. Dennis, and W. Kintsch (eds), *Latent Semantic Analysis: A Road to Meaning*. Laurence Erlbaum.

  [An introduction to multiple context free grammars for linguists]: http://www.cs.rhul.ac.uk/home/alexc/lot2012/mcfgsforlinguists.pdf
  [*Think Python: How to Think Like a Computer Scientist*]: http://greenteapress.com/wp/think-python-2e/
  [Computational Phonology -- Part I: Foundations.]: http://onlinelibrary.wiley.com.ezp.lib.rochester.edu/doi/10.1111/j.1749-818X.2011.00269.x/abstract
  [Tree-adjoining grammars]: https://www.cis.upenn.edu/~joshi/joshi-schabes-tag-97.pdf
  [Foundations of Statistical Natural Language Processing]: http://ics.upjs.sk/~pero/web/documents/pillar/Manning_Schuetze_StatisticalNLP.pdf
  [*Speech and Language Processing*]: http://stp.lingfil.uu.se/~santinim/ml/2014/JurafskyMartinSpeechAndLanguageProcessing2ed_draft%202007.pdf
  [1]: https://web.stanford.edu/~jurafsky/slp3/ed3book.pdf
  [*Introduction to the Theory of Computation*]: https://theswissbay.ch/pdf/Book/Introduction%20to%20the%20theory%20of%20computation_third%20edition%20-%20Michael%20Sipser.pdf
  [An Introduction to Conditional Random Fields]: http://homepages.inf.ed.ac.uk/csutton/publications/crftut-fnt.pdf
  [Computational perspectives on minimalism]: http://linguistics.ucla.edu/people/stabler/Stabler10-Min.pdf
  [Probabilistic Topic Models]: http://psiexp.ss.uci.edu/research/papers/SteyversGriffithsLSABookFormatted.pdf
  [Regular models of phonological rule systems]: https://web.stanford.edu/~mjkay/Kaplan%26Kay.pdf
  [Combinatory Categorial Grammar]: http://lingo.stanford.edu/sag/L222B/papers/Steedman.pdf
