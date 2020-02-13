# This is the journal for Comp sci

1. What did you do?
 We watched video about introduction of computer science. Then we wrote down detailed process of making jam sandwitch in groups of 3.
1. What did you learn?
 I learned how hard it is to write down every single steps of just simple actions.
1. What question do you have?
 None
 


# These variables are to count the rools of the dice

ones=0
twos=0
threes=0
fours=0
fives=0
sixes=0

def setup():
    size (600,600)
    background(255)
    barGraph()
    
def draw():
    x=0
    mouseClick()
    delay(200)
    barGraph()
    
def barGraph():
    global ones
    fill(0)
    textSize(20)
    for x in range(6):
        text(x+1,(50+50*x), 580)
    strokeWeight(5)
    rect(50, 550 - ones, 20, ones)
    rect(100, 550 - twos, 20, twos)
    rect(150, 550 - threes, 20, threes)
    rect(200, 550 - fours, 20, fours)
    rect(250, 550 - fives, 20, fives)
    rect(300, 550 - sixes, 20, sixes)
    
def mouseClick():
    global ones, twos, threes, fours, fives, sixes
    background(255)
    stroke(0)
    fill(255)
    rect(100,100, 400, 400, 10)
    stroke(255,0,0)
    strokeWeight(10)
    
    n=random(0,6)
    if 0<=n<1.0:
        circle(300,300,50)
        ones= ones + 1
        print("number of times one has been rolled:",ones)
    if 1<=n<2.0:
        circle(200,200,50)
        circle(400,400,50)
        twos= twos + 1
        print("number of times two has been rolled:",twos)
    if 2.0<=n<3.0:
        circle(200,200,50)
        circle(400,400,50)
        circle(300,300,50)
        threes= threes + 1
        print("number of times three has been rolled:",threes)
    if 3.0<=n<4.0:
        circle(200,200,50)
        circle(400,200,50)
        circle(200,400,50)
        circle(400,400,50)
        fours= fours + 1
        print("number of times four has been rolled:",fours)
    if 4.0<=n<5.0:
        circle(200,200,50)
        circle(400,200,50)
        circle(200,400,50)
        circle(400,400,50)
        circle(300,300,50)
        fives= fives + 1
        print("number of times five has been rolled:",fives)
    if 5.0<=n<6.0:
        circle(200,200,50)
        circle(400,200,50)
        circle(200,400,50)
        circle(400,400,50)
        circle(200,300,50)
        circle(400,300,50)
        sixes= sixes + 1
        print("number of times six has been rolled:",sixes)
1.What did you do?
We learned how to code a dice. For example, changing color, adding graph counter and changing speed.
1. What did you learn?
I learned how to change color of background and what number represents different colors.
What question do you have?
None
