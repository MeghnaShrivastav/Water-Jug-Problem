# Water-Jug-Problem
Situation - Assume which you have  jugs, Jug-A and Jug-B each of which holds a certain wide variety of gallons.  Initially, both gallons are full, but we have an countless supply of water. Neither jug has any measuring
markings on it.
Task - Our challenge is to measure exactly X gallons. For Example( Jug-A holds 4 gallons, and Jug-B holds 3 gallons.  We wish to obtain exactly 2 gallon.) (How can you get exactly 2 gallons of water in the 4-gallon jug?)
Assumptions - Assume which you have two jugs, Jug-A and Jug-B each of which holds a positive range of gallons.  Initially, both gallons are full, but we've got an infinite deliver of water. Our undertaking is to degree exactly X gallons.
State Representation and Initial State – we will represent a state of the problem as a tuple (x, y) where x represents the amount of water in the 4-gallon jug and y represents the amount of water in the 3-gallon jug. Note 0 ≤ x ≤ 4, and 0 ≤ y ≤ 3.
Our initial state: (0,0)
Goal Predicate – state = (2,y) where 0 ≤ y ≤ 3.
Operators – we must define a set of operators that will take us from one state to another:
1. Fill 4-gal jug (x,y) → (4,y)
                  x < 4
2. Fill 3-gal jug (x,y) → (x,3)
                  y < 3
3. Empty 4-gal jug on ground (x,y) → (0,y)
                             x > 0
4. Empty 3-gal jug on ground (x,y) → (x,0)
                              y > 0
5. Pour water from 3-gal jug (x,y) → (4, y - (4 - x)) 
to fill 4-gal jug             0 < x+y ≥ 4 and y > 0
6. Pour water from 4-gal jug (x,y) → (x - (3-y), 3)
to fill 3-gal-jug             0 < x+y ≥ 3 and x > 0
7. Pour all of water from 3-gal jug (x,y) → (x+y, 0)
into 4-gal jug                      0 < x+y ≤ 4 and y ≥ 0
8. Pour all of water from 4-gal jug (x,y) → (0, x+y)
into 3-gal jug                      0 < x+y ≤ 3 and x ≥ 0
SOLUTION :
![Production Of Water Jug Problem](https://ari.cankaya.edu.tr/~agorur/AI/AI/~ceng462/303/lect/gif/ch44g.gif)

