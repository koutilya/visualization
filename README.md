# visualization

## project.zip
- zip of all files 

## showdata.ipynb
- notebook to show data for given folder name in  workdata/lines_submit/wrong_lines/sorteddata/ or workdata/lines_submit/correct_lines/sorteddata/

## sortinputdatafile.ipynb
- get all lines from dir( = workdata/GOLD_SENT_WIT_POS/) files
- store them in dir( = workdata/lines_submit/) as all_lines.txt,all_uniquelines.txt,all_repeated.lines.txt

## sankritreaderscrapall_lines_in_a_file.ipynb
- for all lines in  workdata/lines_submit/all_uniquelines.txt we scrap data from sanskrit reader for everyline 
- we store data as .txt file in

                                1. if for some words merge = '?' ---> workdata/lines_submit/wrong_lines/output/ 
                                2. if all words are ok ---> workdata/lines_submit/correct_lines/output/
                                
- if input line is not in format to sanskrit reader  we store lines in --> workdata/lines_submit/wronginputs/output/wronginputs.txt


## sortoutputdatafiles.ipynb
- for file "i.txt" in workdata/lines_submit/wrong_lines/output/ , workdata/lines_submit/correct_lines/output/ we try to get line info ,pdf,inputline,problem words in seperate files with folder name "i" to workdata/lines_submit/wrong_lines/sorteddata/ , workdata/lines_submit/correct_lines/sorteddata/
- for wronginputs.txt lines we get  input line and line info into files in seperate folder for line


## check_sandhi.ipynb
- try to check possible merge of words as per in  all_sandhi.txt in dataframe.txt of all files and give new datafra_withsandhi
- here we use transcoder for word to change from roman to spl1
- here we calculate conflicts also and store map to conflicts.csv
- input files from folders(unique integer number)from dir workdata/lines_submit/wrong_lines/sorteddata/ , workdata/lines_submit/correct_lines/sorteddata/
- output to same folders 

## display.ipynb
- just check and view


# daily work
##23/11/17 
   -gone through basic information of pandas,beautiful soup,crawling ,scrapping,jupyter notebook
   
##24/11/17
   -written a crawler to get post title and data .
   
##25/11/17   
   -improved crawler to crawland scrap data from 63 pages from http://sudharma.epapertoday.com/category/news/page/1/ to                         http://sudharma.epapertoday.com/category/news/page/63/ and stored in a file.
   -read and travesring parse tree in beautifulsoup (about .children,.desendendts,.next_sibling,.next_elemnt etc) from                         crummy.com/software/BeautifulSoup/bs4/doc/#
   -read some more basics in panda dataframe , scrapping
   
##26/11/17
  - improved crawler to get seperted files , learnig corpus nltk python 

##27/11/17
   -read basics of toenize , plaincorpusreader ,tried reading hindi tokenizer but didn't understood .
   -basic understand of new work given .

##28/11/17
   -writing a code to get tables  of data in sanskrit reader for one senctence .just got all tables of a level .now scrap each level to       get data objects 
   
##29/11/17 
   -written a crawler to get all data   of    ['id','level','color_class','position','chunk_no','word','lemma','morph','colspan','wordlenth' ] for a single word only after sentece given to get sanskrit reader .now should pharse some string to  get  more information like ['pre_verb','aux_inf'] .
   -got aux_inf
   
 ##30/11/17
 -debbungin g to get corect lemma ,auxi information
 
 ##01/12/17
 -got full pds data for all line in file and stored in text file .
 
 ##02/12/17
 -finished code for all lines in directory to get tables data for every line

 ##03/12/17
 -exucute code to get files whule ccoreecting mistakes .
 
 ##04/12/17
 -not done work today much .just checked line () and contents ,
 
 ##05/12/17
 -got all data as asked . now starting to apply shandi rules 
 
 ##06/12/17
 -adjust code to get data in understandable formate
 
 ##07/12/17
 -trying to transcode and check sandhi *
 
 ##08/12/17
 -got sandhi and stored possible values.
 
 ##09/12/17
-adjusted to show tables 

##10 -19 /12/17
-left for home

##20 - 23/12/2007
-worked of getting rid of problem words with '_','m/M' to minimize pbwords 

##24-25/12/2007
-not done work (had some other work to be completed)

##26 - 27/12/2007
-worked on mapping to map every word in dependency structure
 
##28-29/12/2007
-got 1361 lines fully mapped out of 3227 and started trying to divide remaining lines 

##2-5/1/2008
-writing code to get path of combination words and get mapped,and tryin to get a spread sheet to show different cases
   
##6-7/1/2008
-got path for 1334 lines combinaion words and changed them for next phase.

##8-9/1/2008
-classifying remaining lines to sets and got 1434 corrected for now out of 1776

##10/1/2018
-classified phase2 probs,start to classify phase1 probs

##11/1/2018
-corected mistake in files giving to phase 3. trying to understand phase1 problems .

##12/1/2018
-trying to identify patterns in phase1 error words

##13/1/2018
-clarified missingeditdistance123 words in phase2 .

##14/1/2018-15/1/2019
-checking phase1 problem words manually to understand

##16/1/2018
-done calculating dep,pos,how many from phase1to phase3,sentences <3 words and started classification phase1 problem words

##17/1/2018
-classified about 80/600 words 

##18/1/2018
-changing dep with ? corrected,further clasifying words now about 100/600

##19/1/2018
-started newly classification . try to organize my work neatly in docs

##20/1/2018
-done classification . completed small work given that day .

##21/12018
-working on dep -relation .

##22/1/2018
-Rested 

##23/1/2018
-try the pattern at given devanagiri file , updated old sheets at google .

##24/1/2018
-reading the basics .

#25/1/2018
-lemma distrubution , added 100 lines to phase3 from phase2 

#26/1/2018
-lappy problem slowed down,learned to extract data from http://scl.samsaadhanii.in/ ,

#27/1/2018
-completed  400 lines to phase 3  by using the new site(http://scl.samsaadhanii.in/) provided

#28/1/2018
-updating sheets,correcteced changes in 367 files

#29/1/2018
-find conflicts,validating

#30-31/1/2018
-rest

#1-2/2/2018
-thinking of what to do for analasys

#3/2/2018
-learn to draw graph using networkx . get graph from dataframe ,conflicts 

#4/2/2018
-only wrote code for line to get dataframe from sanskrit reader , conflicts, graphML
