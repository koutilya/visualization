# in zip files  of wrong_lines ,correct_lines,wronginputs
## /output/
- data get from scrapper for each line

## /sorteddata/.*/
- original.txt store line,its analasys,with original file name
- inputline.txt store input line to site .
- problem.txt store problem words
- dataframe.txt stores dataframe of ech lines
- dataframe_withsandhi.txt stores possible words and inxexs for given word in a seperate column .it also has extra column for slp1 translation of word which is in roman
- conflicts.csv is a map of [index][index] of dataframe  where 0 = not conflict, 1 = can merge , 2  = conflict
