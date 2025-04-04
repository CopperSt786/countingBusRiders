**Counting Bus Riders**

[ Memory: 64 MB, CPU: 1 sec ]

Farmer John has taken a second job as a bus driver to help cover his farm’s massive budget deficit. He starts his shift with some unknown number of people on the bus and he ends his shift with some unknown number of people on the bus.

He was supposed to record both of these pieces of information, but was too focused on driving to keep accurate records. Instead, he has the following information:

Each time people got off the bus, he recorded that between X and Y people left the bus. In FJ’s notes, this appears as “off X Y”. 

Each time people got on the bus, he recorded that between X and Y people entered the bus. In FJ’s notes, this appears as “on X Y”.

Occasionally, Farmer John recorded that there were between X and Y people on the bus. In FJ’s notes, this appears as “none X Y”

In total, Farmer John made N (1 <= N <= 100) of these readings. Using Farmer John’s notes, determine the minimum and maximum number of people who started on the bus when Farmer John’s shift began and the minimum and maximum number of people still on the bus when Farmer John’s shift ended.
<br>
INPUT FORMAT:

Line 1: N, the number of records Farmer John made.
Lines 2…N+1: A string (off, on, or none) and two integers X and Y (0 <= X, Y <= 1000). It is guaranteed that at least one of these readings will start with “none”.

Note that the inputs appear in chronological order. So the reading in line 2 was made before the reading in line 3 and so on.

OUTPUT FORMAT:

Line 1: Two integers: the minimum and maximum number of people on the bus when Farmer John’s shift started
Line 2: Two integers: the minimum and maximum number of people on the bus when Farmer John’s shift ended
<br>
<br>
<br>
SAMPLE INPUT:
    
    4
    off 2 2
    none 5 7
    none 6 10
    on 3 5
    
SAMPLE OUTPUT:

    8 9
    9 12

In this example, the none readings tell us that there are between 6 and 7 people on the bus before the people at the start got off the bus and the people at the end got on the bus. Before this, the off reading tells us that exactly 2 people got off the bus, so 8 to 9 people must have started on the bus. After this, the on reading tells us that 3 to 5 people got on the bus, so there must be between 9 and 12 people on the bus.
<br>
<br>
<br>

MODE: normal<br>
Language <br>
cpp<br>


