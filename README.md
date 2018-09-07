#For_parser
#gbxml, ifcxml files to use in GeoLinked_HollyFerguson code

#Add file path as inputfile in Holly's GeoLinked_HollyFerguson code and run to produce graph --> gets put in FinalGraph folder as MyGraph.ttl (for debugging purposes this is all you need)
#For Resilience_Orchestration bundle (1) Run GeoLinked_HollyFerguson with inputfile of choice (2) Change inputfileIFCXML variable in Resilience_Orchestration's main.py file (around line 122) 
#To query the SGraph within Resilience_Orchestration bundle, will need to specify file path for outputfile variable (inside Query Semantic Graph section in main.py around line 150)

#Information about input files I am providing:
#RC_FRAME_CMU_walls.ifcxml --> runs w/o problems (gives me all spatial information for walls/floors and columns (beams have to be done separately...requires visibility changes in Revit and another ifcxml file)
#RC_FRAME_CMU_walls.xml --> (from Revit 2016) gbxml used in GreenScale, produces an xpath error

#Sample files within Holly's GeoLinked_HollyFerguson code
#gbxmls
#Files that run w/o problems and give back strings with material names and associated thicknesses
#4_Room_GBXML.xml (Revit 2013)
#4Room_RoundColumns_GBXML.xml (Revit 2014) 
#4Room_SquareColumns_GBXML.xml (Revit 2014)
#Single_Room_GBXML.xml (Revit 2014)

#Files that give back xpath error (something in the structureAddon.py file) 
#4Room2014_gbxml_WFlange.xml (Revit 2014) 
#4Room2016_gbxmlWFlange.xml (Revit 2016) 
#L_1Floor_GBXML.xml (Revit 2014)
#L_2Floor_GBXML.xml (Revit 2014)
#Vet_Center_GBXML.xml (Revit 2014)
