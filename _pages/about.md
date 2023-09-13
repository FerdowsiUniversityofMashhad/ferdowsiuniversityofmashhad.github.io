---
permalink: /
title: "academicpages is a ready-to-fork GitHub Pages template for academic personal websites"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

This is the front page of a website that is powered by the [academicpages template](https://github.com/academicpages/academicpages.github.io) and hosted on GitHub pages. [GitHub pages](https://pages.github.com) is a free service in which websites are built and hosted from code and data stored in a GitHub repository, automatically updating when a new commit is made to the respository. This template was forked from the [Minimal Mistakes Jekyll Theme](https://mmistakes.github.io/minimal-mistakes/) created by Michael Rose, and then extended to support the kinds of content that academics have: publications, talks, teaching, a portfolio, blog posts, and a dynamically-generated CV. You can fork [this repository](https://github.com/academicpages/academicpages.github.io) right now, modify the configuration and markdown files, add your own PDFs and other content, and have your own site for free, with no ads! An older version of this template powers my own personal website at [stuartgeiger.com](http://stuartgeiger.com), which uses [this Github repository](https://github.com/staeiou/staeiou.github.io).

A data-driven personal website
======
Like many other Jekyll-based GitHub Pages templates, academicpages makes you separate the website's content from its form. The content & metadata of your website are in structured markdown files, while various other files constitute the theme, specifying how to transform that content & metadata into HTML pages. You keep these various markdown (.md), YAML (.yml), HTML, and CSS files in a public GitHub repository. Each time you commit and push an update to the repository, the [GitHub pages](https://pages.github.com/) service creates static HTML pages based on these files, which are hosted on GitHub's servers free of charge.

Many of the features of dynamic content management systems (like Wordpress) can be achieved in this fashion, using a fraction of the computational resources and with far less vulnerability to hacking and DDoSing. You can also modify the theme to your heart's content without touching the content of your site. If you get to a point where you've broken something in Jekyll/HTML/CSS beyond repair, your markdown files describing your talks, publications, etc. are safe. You can rollback the changes or even delete the repository and start over -- just be sure to save the markdown files! Finally, you can also write scripts that process the structured data on the site, such as [this one](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.ipynb) that analyzes metadata in pages about talks to display [a map of every location you've given a talk](https://academicpages.github.io/talkmap.html).

Getting started
======
1. Register a GitHub account if you don't have one and confirm your e-mail (required!)
1. Fork [this repository](https://github.com/academicpages/academicpages.github.io) by clicking the "fork" button in the top right. 
1. Go to the repository's settings (rightmost item in the tabs that start with "Code", should be below "Unwatch"). Rename the repository "[your GitHub username].github.io", which will also be your website's URL.
1. Set site-wide configuration and create content & metadata (see below -- also see [this set of diffs](http://archive.is/3TPas) showing what files were changed to set up [an example site](https://getorg-testacct.github.io) for a user with the username "getorg-testacct")
1. Upload any files (like PDFs, .zip files, etc.) to the files/ directory. They will appear at https://[your GitHub username].github.io/files/example.pdf.  
1. Check status by going to the repository settings, in the "GitHub pages" section

Site-wide configuration
------
The main configuration file for the site is in the base directory in [_config.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_config.yml), which defines the content in the sidebars and other site-wide features. You will need to replace the default variables with ones about yourself and your site's github repository. The configuration file for the top menu is in [_data/navigation.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_data/navigation.yml). For example, if you don't have a portfolio or blog posts, you can remove those items from that navigation.yml file to remove them from the header. 

Create content & metadata
------
For site content, there is one markdown file for each type of content, which are stored in directories like _publications, _talks, _posts, _teaching, or _pages. For example, each talk is a markdown file in the [_talks directory](https://github.com/academicpages/academicpages.github.io/tree/master/_talks). At the top of each markdown file is structured data in YAML about the talk, which the theme will parse to do lots of cool stuff. The same structured data about a talk is used to generate the list of talks on the [Talks page](https://academicpages.github.io/talks), each [individual page](https://academicpages.github.io/talks/2012-03-01-talk-1) for specific talks, the talks section for the [CV page](https://academicpages.github.io/cv), and the [map of places you've given a talk](https://academicpages.github.io/talkmap.html) (if you run this [python file](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.py) or [Jupyter notebook](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.ipynb), which creates the HTML for the map based on the contents of the _talks directory).

**Markdown generator**

I have also created [a set of Jupyter notebooks](https://github.com/academicpages/academicpages.github.io/tree/master/markdown_generator
) that converts a CSV containing structured data about talks or presentations into individual markdown files that will be properly formatted for the academicpages template. The sample CSVs in that directory are the ones I used to create my own personal website at stuartgeiger.com. My usual workflow is that I keep a spreadsheet of my publications and talks, then run the code in these notebooks to generate the markdown files, then commit and push them to the GitHub repository.

How to edit your site's GitHub repository
------
Many people use a git client to create files on their local computer and then push them to GitHub's servers. If you are not familiar with git, you can directly edit these configuration and markdown files directly in the github.com interface. Navigate to a file (like [this one](https://github.com/academicpages/academicpages.github.io/blob/master/_talks/2012-03-01-talk-1.md) and click the pencil icon in the top right of the content preview (to the right of the "Raw | Blame | History" buttons). You can delete a file by clicking the trashcan icon to the right of the pencil icon. You can also create new files or upload files by navigating to a directory and clicking the "Create new file" or "Upload files" buttons. 

Example: editing a markdown file for a talk
![Editing a markdown file for a talk](/images/editing-talk.png)

The History of Ferdowsi University of Mashhad
------
The first proposal for launching the Ferdowsi University of Mashhad was announced concurrently with the establishment of Tehran University in 1934. However, the first step was converting the Higher Institute of Public Health to a Medical Faculty in 1949. Shortly after, the Medical Faculty admitted its first group of medical students, and in December 1949 this institute was officially inaugurated as the first Center for Medical Sciences in the North East of Iran by the Minister of Culture, the late Dr. Zanganeh. Finally in 1956 after the foundation of the facultys of Literature and Theology, the complex was named "Mashhad University". Later on in 1957, the rules and regulations for employment and education of Tehran University were adopted for use in this new university.

Since then other faculties have been gradually added to the university based on the local demand. These are the Faculty of Science (1961), the Faculty of Education, the Faculty of Agriculture (1973), the Faculty of Engineering (1975), the Faculty of Economics and Administrative Sciences (1987), the Faculty of Veterinary Medicine (1991), the Faculty of Mathematics (1996), the Faculty of Architecture, the Faculty of Urbanism and Islamic Arts, and the Faculty of Natural Resources and Environment (2001). In 1975 after the separation of the facultys related to the Medical Sciences from the university, the name of the university was changed from "Mashhad University” to "The Ferdowsi University of Mashhad".

The Ferdowsi University of Mashhad has now nearly seven decades of brilliant educational, research and cultural history and it is well known among institutes of higher education in Iran. It is currently one of the nation’s top three universities and also the largest center of higher education in the North East of Iran.

At present, the Ferdowsi University of Mashhad is composed of 12 facultys, 38 research centers, 7 centers of excellence, 820 faculty members (%50 of whom are professors or associate professors), over 20000 students (9996 undergraduate, 6143 Masters, and 3905 Ph.D. students), and 1050 staff members.

Currently, 1279 foreign students are enrolled in different academic programs at the Ferdowsi University of Mashhad. In addition, there are also 187 foreign students who are passing their six-month training courses in language at the International Center for Teaching Persian to Non-Persian Speakers. These students would begin their academic education after they pass this six-month course of study.

University Honors
List of distinguished people from the Ferdowsi University of Mashhad:

Dr. Ali Shariati, Distinguished faculty member of History
Professor Mohammad Taghi Fatemi, Professor of Mathematics
Dr. Ali Akbar Fayyaz, Professor of Persian Language and Literature
Dr. Gholam Hossein Yousefi, Professor of Persian Language and Literature
Dr. Sayyed Jalal al-Din Ashtiyani, Professor of Islamic Philosophy
Dr. Kazem Modir-Shanechi, Professor of Quranic Sciences and Hadith
Dr. Mohammad Vaezzadeh, Professor of Quranic Sciences and Hadith
 The Distinguished Professors of the University
Late Dr. Hossein Razmjoo, Department of Persian Language and Literature
Late Dr. Mohammad Ali Rajaee Bokharaee, Department of Persian Language and Literature
Late Dr. Lotf-Allah Mafakham Payan, Department of Geography
Late Dr. Sayyed Mohammad Taghi Edalati Sharbaf, Department of Physics
Late Javad Hadidi, Department of French Language and Literature
Dr. Sayyed Mohammad Alavi Moghaddam, Department of Persian Language and Literature
Dr. Rampoor Sadr Nabavi, Department of Social Sciences
Dr. Afzal Forooghi, Department of French Language and Literature
Dr. Rahmatollah Fattahi, Department of Information Sciences and Knowledge Studies
Dr. Gholam-Hossein Haghniya, Department of Soil sciences
Dr. Elaheh Kafshdar Goharshadi, Department of Chemistry
Dr. Mohammad Sal Moslehiyan, Department of Pure Mathematics
Dr. Mohammad-Reza Taraghiyan, Department of Applied Mathematics
Dr. Naser-Reza Arghami, Department of Applied Mathematics
Educational Awards
 Winner of the National Award for Outstanding Student by a student from the Ferdowsi University of Mashhad, August 2015
 Achieving the first rank in the National Nano Competition of Iran at the Bachelor’s level, September 2015
 The best Award winner poster at the International Conference on Nano in Mashhad, June 2015
 Award winner of two bronze medals at the Chemistry Olympiad in the 20th Scientific Student Olympiad, August 2015
 Achieving the first rank in the National Sheikh-Bahai Techno-preneurship Festival, May, 2015
 Achieving the second rank in the 16th National Statistics Students’ Competition by the students’ team of the Faculty of Mathematics, September, 2015
 Achieving the first rank at the National Robotic Competition by the robotics team of the Faculty of Engineering, September, 2015
 Achieving the third rank at the 19th Student Scientific Olympiad, September, 2014
 Achieving the third rank in practical projects of the Khwarizmi International Awards, 2014
 Achieving the first and the second ranks in the Robotic League, March, 2014
 Achieving the first rank at the 19th National Chemistry Olympiad, August, 2014
 Achieving the second rank at the 19th Scientific Student Olympiad, September, 2014
 Award winner of the best doctoral thesis, September, 2013
 Achieving the first and the third ranks at the 18th Scientific Student Olympiad, October, 2013

Research Honors
Achieving the 3rd rank 3 in Iran, 95th in Asia, 455th in world based on the 4ICU Ranking, 2015
Award winner of the Dehkhoda Medal for 2 faculty members of the Ferdowsi University of Mashhad, December, 2015
The Ferdowsi University of Mashhad ranked in the top one percent of the world's influential universities, July, 2015
Developing the technical knowledge of reproducing one of the world’s top five flowers by researchers, August, 2015
Acknowledging two faculty member of the Department of Chemistry as Iran’s prominent chemists, September, 2015
Achieving the third and the fourth ranks in modern languages and chemical engineering based on QS ranking 2014
Achieving the sixth rank among universities affiliated with the Ministry of Science based on URAP ranking system, 2014
Paying tributes to three distinguished faculty members of Geology as Iran’s Top Scientists, October, 2013
Achieving the first rank in the 20th Student Yearbook Festival in the field of Art and Architecture, December, 2013
Honors in Research and Technology
 Achieving the first rank in innovation by the “Rekab Sabz” team of the Faculty of Engineering, March, 2016
Achieving the third rank in ACM International Collegiate Programming Contest by the programming team of the Computer Department, January, 2016
POD system at the Ferdowsi University of Mashhad won a Silver FAB Award, June, 2015
Achieving the first rank at the 5th Communication and IT Festival, May, 2015
Achieving the First rank at the Web Iran Festival, December, 2015
Achieving the second national rank in the Web page size index based on SCIMAGO, 2014
Achieving the third rank at the 4th Communication and Technology Festival in the field of Information, May 2014
Achieving a top rank in simulation lab among 8 top teams in the RoboCup World Championship, August 2015
 Culture and Sport Achievements
Achieving championship at the13th Male Cultural-sports Olympiad, September 2016
Achieving the second rank at the 13th Female Cultural-sports Olympiad, September 2016
Achieving championship at the Public Sports Olympiad of Girls, September 2015
Achieving the rank of outstanding consulting center of Iran by the Consulting Center of the Ferdowsi University of Mashhad, March 2016
Winning 11 outstanding titles by the Art and Cultural Center of the Ferdowsi University of Mashhad in the Rooyesh Festival, June 2015
Winning the title of outstanding lady of Khorasan Razavi by a faculty member, April 2015
Achieving the championship at the12th Male Cultural-sports Olympiad, September 2014
Achieving the second rank at the 12th Female Cultural-sports Olympiad, September 2014
Achieving the first rank in cultural activities of Iranian universities, 2013
Achieving the 11th top ranks in the Quran competitions of region 3, May 2013
Achieving the first, the second and third ranks in the Quran Festival of Iran, October 2013
Achieving the 5 top ranks at the Khwarizmi Festival in the field of student press, May 2013
Achieving the 4 top ranks at the 7th international Festivals of Press and News agencies, May 2013
Achieving the 4 top ranks at the Quran competitions of faculty members, July 2013
Winner of 9 top titles for Art and Cultural Centers at the Ferdowsi University of Mashhad, March 15, 2013
Winner of 8 top titles at the Motion Festival, December 2011
Achieving the third rank at the Students’ National Quran Competition, May 2011
