# Overview
This Java project deals with football league tables.

For each team, the above table shows the number of games Played (P) and, of those, the number of games Won (W), Drawn (D) and Lost (L); then the number of goals scored FOR the team (F) and AGAINST the team (A), and finally the Points (Pt).

My Java code represents a league table by means of two classes: Team Class and League Class.

Notice that the Team class has six instance variables, i.e. name, won, drawn, lost, goalsFor and goalsAgainst, as well as setter methods for all variables except name. There is no setter method for name because it is set once and for all by the constructor when a Team object is created. In addition, there are getter methods for all the instance variables, and methods for returning the number of games played, the goal difference and the points, all of which can be calculated from the values of the instance variables.

The League class declares two instance variables, name and teams (an array of Team objects). It has a constructor, which sets the league’s name to reference the constructor's String argument, and sets the teams to reference an array whose size is the second argument of the constructor. This constructor is declared to be private. This means that it is not possible to create a new League object by invoking the constructor directly from the Workspace. Instead, The League Class will have a class method called loadLeague() whose purpose is to create a new League object, by using the constructor, then fill it with the teams whose details are contained in a text file.
