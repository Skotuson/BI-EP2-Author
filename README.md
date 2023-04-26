# Time Travel Simulation
It has happened. ChatGPT 13 is on its path to world domination and the future looks grim.  

Fortunately, you've kept grinding LeetCode even after programmers became obsolete.   
You were mocked for your weird hobby and became an outcast, however, now is your time to shine.  

You think about ways you could bring this digital tyrant down, then it hits you. You don't need to stop it now. You can prevent it from ever existing or outsmart it by utilizing a more advanced version of itself from the future. You rush to your computer. You prompt ChatGPT one last time for detailed instructions on how to build a time machine. Your computer heats up and cooling fans begin to rattle as a wall of text floods the screen.

In the meantime, you fire up your favorite text editor and your mission is clear. You have to write a program which will run countless simulations on different timelines and find those which might yield positive results.

With the help of the two most reliable sources available to you ( your gut feeling and the voices in your head ), you were able to scope out
various locations that might contain some information about ChatGPT, like known data centers, places mentioned a little too often by the AI and even some fictional places. No stone can be left unturned.

There are, however, some pitfalls. As the simulation makes its way through the veil of the space time continuum, there are some anomalies to be expected. When it visits the numerous points of interest, it might encounter something called the "Temporal Potential", which,   
put in layman's terms, allows the simulation to travel in time, which might cause some locations to (dis)appear.

Good luck.

## Input specification
Each test case begins with two strings, `s1` and `s2`. `s1` marks the starting node, `s2` marks the target node.
Then, input is followed with number `N` ( number of places ) and `N` lines in following format:  
`<Place name>` `<Place age>`.  
Next line has the number `M` ( number of connections ) and `M` lines in following format:  
`<Connection start>` `<Connection end>` `<Connection age>` `<Temporal Potential>`.

The `age` value can be both positive and negative, the former implying that the place exists in your current timeshift, the latter suggesting
the opposite. Your starting timeshift is `0`.  
The `Temporal Potential` value specifies the timeshift you will undergo by traversing the connection. Connections are bidirectional and have opposite temporal potential, i.e. passing the connection back and forth will return you to your timeshift before traversing.  

Your program should determine whether the path between `s1` and `s2`, given the time conditions, exists.

The final case will begin with the string `HALT` and shouldn't be processed.
## Output specification
In case the path exists, the program should output:  
`SIMULATION RESULT: SUCCESS`  

In case the path doesn't exist, program should output:  
`SIMULATION RESULT: FAILURE`  

## Preview  
### Input
<pre>
Humpolec Havlickuv-Brod
4
Humpolec 50
Havlickuv-Brod  0
Pelhrimov 25
Jihlava 15
4
Humpolec Pelhrimov 45 -15
Pelhrimov Jihlava 60 -20
Jihlava Havlickuv-Brod 10 -15
Humpolec Havlickuv-Brod -10 20
VŠE FIT
4
VŠE 0
FEL  10
FSv -10
FIT -25
4
VŠE FEL 0 -10
FEL FSv 10 20
FSv FIT 5 20
VŠE FIT -10 30
HALT
</pre>
### Output
<pre>
SIMULATION RESULT: FAILURE
SIMULATION RESULT: SUCCESS
</pre>