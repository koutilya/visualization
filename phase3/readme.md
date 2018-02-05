# main files are dataframe_towork.csv,conflicts_towork.csv,Graph_towork.graphml,input_line.txt,dependency.txt,original_line.text

# In conflicts_towork 
  note conflicts for 2 ids in dataframe_towork
  take 'id' column as index .
  1 = conflict
  0 = notconflict
  2 = just placed for itself .(ie diagnal values = 2 in dataframe).
  
# In Dataframe_towork

  wordorder column contains word order from dependency tree
  
  
  
# Graph_towork.graphml
  Here we take every row in Dataframe_towork as node with attributes .
  Here every edge represent two nodes(i.e rows in Dataframe_towork) which are not conflicted .
  
  
# folder 999 
  Is sample of all my files in phase3.zip  .
