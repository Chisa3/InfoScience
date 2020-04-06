# 1. This is the journal for Comp sci

1. What did you do?
 We watched video about introduction of computer science. Then we wrote down detailed process of making jam sandwitch in groups of 3.
1. What did you learn?
 I learned how hard it is to write down every single steps of just simple actions.
1. What question do you have?
 None

# 2. These variables are to count the rools of the dice

 1. What did you do?
 We learned how to code a dice. For example, changing color, adding graph counter and changing speed.
 1. What did you learn?
 I learned how to change color of background and what number represents different colors.
 1. What question do you have?
 None
 
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

 # 3. Creating illusion
 1. What did you do?
 As a class we created a suare illusion together.
 I start creating Ehrenstein's square illusion, I started with coding lots of circles in different sizes like it has on the orginal
 illusion. I also created square inside those circles. Although I'm still working on making the square transparent.
 1. What did you learn?
 I learned to to create circles in different sizes in processing and how to foing cordinates for squares as the square had to fit in the circle perfectly.
1. What question do you have?
I want to know how to fill the color of square with transparent.

    offset = 50
    def mouseClicked():
    global offset
    offset = offset + 1 
  
    def setup():
    size (500,500)
    background(255)
    
    def draw():
    stroke(0) # lines are black
    y = 50
    for inc in range(9):
       line(0, y, 500, y)
       y = y + 50
       
    fill(0)
    stroke(255)
    y = 0
    for rows in range(5):
        x = 0
    for rep in range(5):
            square(x, y, 50)
            x = x + 100
        y = y + 100
        
    y = 50 # start of the even rows 
    global offset 
    for rows in range(5): 
        x = 0 + offset 
        for rep in range(5):
            square(x, y, 50)
            x = x + 100
        y = y + 100


 # 4. Creating your illusion and make presentation
 1. What did you do?
 I finished coding Ehrenstein's square illusion. I found out how to make the square transparent and chose to change size of the square as
 it was too small. I also made the square inside the circles to be able to change size when I click.
 1. What did you learn?
 I learned how to code squares that change it's size when I click.


    radius=20
    def setup():
    size(500,500)
    circles()
    
    def circles ():
    background(255)
    strokeWeight(3)
    circle(250,250,300)
    circle(250,250,280)
    circle(250,250,260)
    circle(250,250,240)
    circle(250,250,220)
    circle(250,250,200)
    circle(250,250,180)
    circle(250,250,160)
    circle(250,250,140)
    circle(250,250,120)
    circle(250,250,100)
    circle(250,250,80)
    circle(250,250,60)
    circle(250,250,40)
    circle(250,250,20)

    def draw():
    pass

    def mouseClicked ():
    global radius
    circles()
    radius=radius+10
    fill(255,0,0,0)
    x=250-radius*0.707
    y=250-radius*0.707
    print (x,y)
    square(x,y,2*radius*0.707)

# 5. Tasks for week 28

Veideo 1 - Representing Individuals
   # bounderies conditions
        if x[i] > 500: 
            x[i] = 500 # right
        if y[i] > 500:
            y[i] = 500 # bottom
        if y[i] < 0:
            y[i] = 0 # top
        if x[i] < 0: 
            x[i] = 0 # left
  
  Video 2 - Representing a community
