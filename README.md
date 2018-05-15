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


