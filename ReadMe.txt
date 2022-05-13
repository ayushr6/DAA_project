github link: https://github.com/ayushr6/DAA_project.git

# Problem Statement

Web mapping consumer application like Google Maps offered by Google is quite popular and helpful nowadays as it enables us to 
find the shortest path from one specific location to another, despite the case we are walking, biking, driving or using any 
public transport. It eventually helps us to pan our route effortlessly. But, the question is, what sort of algorithm is behind 
this world’s most popular functionality? Not the actual implementation, but we have tried to find the shortest path between two 
districts between states Rajasthan, Punjab and Gujarat.


# Data Formation

We have used Google Maps to get distance between two districts (by road distance).
We have connect all districts with its neighbouring districts in graph as nodes. For e.g. we have connected Jaipur with districts 
which shares their border with Jaipur. With districts of three states, we got a matrix of 89 x 89. 
Punjab - 23 districts
Rajasthan - 33 districts
Gujarat - 33 districts


# Matrix Example

0	     Amritsar	Barnala	   Bathinda	Faridkot
Amritsar	0	   0	      0		   0
Barnala		0	   0	      65           0
Bathinda	0	   65	      0	      	   70
Faridkot	0	   0	      70	   0


# Algorithm Implemented

To find the shortest path between two nodes (districts) we have used Dijkstra algorithm (Greedy Algorithm). At every step of the 
algorithm, we find a node that is connected to a node (starting with source) and has a minimum distance from that node or have 
minimum edge weight. After getting the path with minimum cost (kilometers), we display the path, from source to destination,i.e., 
from which districts one is required to travel to reach his/her destination with minimum cost.


# Result

Enter District Name (Source): 
Amritsar
Enter District Name (Destination): 
Jaipur
Source: Amritsar
Destination: Jaipur
Cost (Km): 727.0 Km
Path: -> Amritsar -> Tarn Taran -> Firozpur -> Fazilka -> Hanumangarh -> Churu -> Sikar -> Jaipur 


# Team Members

  Ayush Ranwa (2020BTechCSE016)
  Ritisha Mathur (2020BTechCSE065)
  Yash Agarwal (2020BTechCSE102) 
