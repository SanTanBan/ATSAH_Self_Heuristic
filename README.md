# SelfHeuristic
Extremely fast Heuristic for solving mVRPSDP with limited number of Vehicles for each Vehicle Type from a single Depot. Best for Emergency Response. Gives much better solutions than ATS or HLS.


To check with some sample data... Download any of the Data folders. Two Data for 35 Nodes and 150 Nodes are provided...



After that keep all the Python Files in that same folder of the Data and run the MainPython file...

The solutions will be automatically generated within a folder... Change the number of instances within the MainPython file...

Number of instances refer to the number of times the ATSAH will be called for 1 DataSet...

For the 150 Nodes Data; The Number of Vehicles for each Vehicle Types will need to be increased to obtain feasible solutions...



To allow much better solutions increase the f_iter in the ATSAH file to:-

f_iter=len(Node_Sequence)*33

This will only increase the number of times the outerloop is called and therefore will force the Heuristic to try harder and stop much later; although this would only increase the time by about 99 times
