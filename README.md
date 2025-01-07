# Trivia-Game
# Game Code
# Main Menu/step 0
def main_menu():
    global step, button
    background(229,204,255)
    fill(51, 0, 102)
    rect(200,400,100,50) # start button 
    textSize(40)
    fill(51,0,102)
    text("Are you a",150,170)
    text("Trivia Master?",110,230)
    textSize(32)
    fill(229,204,255)
    text("Start", 210,440)

    if button == 1:
        step = 1
        button = 0 # reset button

#game level 1/step 1
def game():
    global step, button
    background(175,238,238)
    #question
    textSize(40)
    fill(0,0,255)
    text("Which is the fastest ",50,110)
    text("animal?", 180,150)
    #drawing the buttons and text
    fill(0,0,255)  #button 2 color
    rect(45,410,150,50) #button 2 bottom left
    fill(0,0,255)  #button 3 color
    rect(300,410,150,50) # button 3 bottom right
    fill(0,0,255)   #button 4 color
    rect(45,250,150,50)  #button 4 top left
    fill(0,0,255)   #button 5 color
    rect(300,250,150,50)  #button 5 top right
    fill(175,238,238) 
    textSize(32)
    text("Cheetah",55,450) #button 2 bottom left
    text("Snake",320,450)  # button 3 bottom right
    text("Cat",80,290) #button 4 top left
    text("Lion",340,290)  #button 5 top right

    if button == 2:
        step = 2
        button = 0
    elif button == 3 or button == 4 or button == 5:
        step = 3
        button = 0
    else:
        pass

#game level 2/step 4
def game2():
    global step, button
    background(175,238,238)
    #question
    textSize(40)
    fill(0,0,255)
    text("How many sides does",40,110)
    text("a Octagon have?",110,150)
    #drawing buttons and text
    fill(0,0,255)  #button 2 color
    rect(45,410,150,50) #button 2 bottom left
    fill(0,0,255)  #button 3 color
    rect(300,410,150,50) # button 3 bottom right
    fill(0,0,255)   #button 4 color
    rect(45,250,150,50)  #button 4 top left
    fill(0,0,255)   #button 5 color
    rect(300,250,150,50)  #button 5 top right
    textSize(32)
    fill(175,238,238)
    text("Four",80,450) #button 2 bottom left
    text("Ten",345,450)  # button 3 bottom right
    text("Five",80,290) #button 4 top left
    text("Eight",335,290)  #button 5 top right

    if button == 5:
        step = 5
        button = 0
    elif button == 2 or button == 3 or button == 4:
        step = 6
        button = 0

#game level 3/step 7
def game3():
    global step, button
    background(175,238,238)
    #question
    textSize(40)
    fill(0,0,255)
    text("What is the biggest",45,110)
    text("country in the world?",40,150)
    #drawing buttons and text
    fill(0,0,255)  #button 2 color
    rect(45,410,150,50) #button 2 bottom left
    fill(0,0,255)  #button 3 color
    rect(300,410,150,50) # button 3 bottom right
    fill(0,0,255)   #button 4 color
    rect(45,250,150,50)  #button 4 top left
    fill(0,0,255)   #button 5 color
    rect(300,250,150,50)  #button 5 top right
    textSize(32)
    fill(175,238,238)
    text("Canada",60,450) #button 2 bottom left
    text("Russia",325,450)  # button 3 bottom right
    text("Australia",52,290) #button 4 top left
    text("America",310,290)  #button 5 top right

    if button == 3:
        step = 8
        button = 0
    elif button == 2 or button == 4 or button == 5:
        step = 9
        button = 0

#game level 4/step 10
def game4():
    global step, button
    background(175,238,238)
    #question
    textSize(40)
    fill(0,0,255)
    text("Where is the Eiffel",55,110)
    text("Tower located?",100,150)
    #drawing buttons and text
    fill(0,0,255)  #button 2 color
    rect(45,410,150,50) #button 2 bottom left
    fill(0,0,255)  #button 3 color
    rect(300,410,150,50) # button 3 bottom right
    fill(0,0,255)   #button 4 color
    rect(45,250,150,50)  #button 4 top left
    fill(0,0,255)   #button 5 color
    rect(300,250,150,50)  #button 5 top right
    textSize(32)
    fill(175,238,238)
    text("France",65,450) #button 2 bottom left
    text("America",310,450)  # button 3 bottom right
    text("Turkey",60,290) #button 4 top left
    text("China",320,290)  #button 5 top right

    if button == 2:
        step = 11
        button = 0
    elif button == 3 or button == 4 or button == 5:
        step = 12
        button = 0

#game level 5/step 13
def game5():
    global step, button
    background(175,238,238)
    #question
    textSize(40)
    fill(0,0,255)
    text("Who built the ",110,110)
    text("Pyramids?",140,150)
    #drawing buttons and text
    fill(0,0,255)  #button 2 color
    rect(45,410,150,50) #button 2 bottom left
    fill(0,0,255)  #button 3 color
    rect(300,410,150,50) # button 3 bottom right
    fill(0,0,255)   #button 4 color
    rect(45,250,150,50)  #button 4 top left
    fill(0,0,255)   #button 5 color
    rect(300,250,150,50)  #button 5 top right
    textSize(26)
    fill(175,238,238)
    text("The Queen",50,450) #button 2 bottom left
    text("Egyptians",310,450)  # button 3 bottom right
    textSize(32)
    text("Vikings",65,290) #button 4 top left
    text("Romans",310,290)  #button 5 top right

    if button == 3:
        step = 14
        button = 0
    elif button == 2 or button == 4 or button == 5:
        step = 15
        button = 0


#text and buttons for winner functions
def winnertxt():
    global step, button
    background(127,255,212)
    textSize(60)
    fill(46,139,87)
    text("CORRECT!",95,180)
    rect(40,310,175,50)  # next level button 6
    rect(290,310,145,50)  #quit button 7
    textSize(32)
    fill(127,255,212)
    text("Next Level",45,350)
    text("Quit",325,350)

#win screen 1/step 2
def winner():
    global button, step
    winnertxt()
    textSize(32)
    fill(46,139,87)
    text("1/10",420,35)
    if button == 6:
        step = 4
        button = 0
    elif button == 7:
        step = 0
        button =0

#win screen 2/step 5
def winner2():
    global button, step
    winnertxt()
    textSize(32)
    fill(46,139,87)
    text("2/10",420,35)
    if button == 6:
        step = 7
        button = 0
    elif button == 7:
        step = 0
        button =0

#win screen 3/step 8
def winner3():
    global button, step
    winnertxt()
    textSize(32)
    fill(46,139,87)
    text("3/10",420,35)
    if button == 6:
        step = 10
        button = 0
    elif button == 7:
        step = 0
        button =0

#win screen 4/step 11
def winner4():
    global button, step
    winnertxt()
    textSize(32)
    fill(46,139,87)
    text("4/10",420,35)
    if button == 6:
        step = 13
        button = 0
    elif button == 7:
        step = 0
        button =0

#win screen 5/step 14
def winner5():
    global button, step
    winnertxt()
    textSize(32)
    fill(46,139,87)
    text("5/10",420,35)
    if button == 6:
        step = 16
        button = 0
    elif button == 7:
        step = 0
        button = 0


    
#text and buttons for the loser functions
def losertxt():
    background(255,160,122)
    textSize(60)
    fill(255,0,0)
    text("INCORRECT!",60,180)
    fill(255,0,0)
    rect(40,310,175,50)  #try again button 6
    rect(290,310,140,50)  #give up button 7
    textSize(32)
    fill(255,160,122)
    text("Try Again?",45,350)
    text("Give up",300,350)

#loser screen 1/step 3
def loser():
    global button, step
    losertxt()
    if button == 6:
        step = 1
        button = 0
    elif button == 7:
        step = 0
        button = 0

#loss screen 2/step 6
def loser2():
    global button, step
    losertxt()
    if button == 6:
        step = 4
        button = 0
    elif button == 7:
        step = 0
        button = 0

#loss screen 3/step 9
def loser3():
    global button, step
    losertxt()

    if button == 6:
        step = 7
        button = 0
    elif button == 7:
        step = 0
        button = 0

#loss screen 4/step 12
def loser4():
    global button, step
    losertxt()

    if button == 6:
        step = 10
        button = 0
    elif button == 7:
        step = 0
        button = 0

#loss screen 5/step 15
def loser5():
    global button, step
    losertxt()

    if button == 6:
        step = 13
        button = 0
    elif button == 7:
        step = 0
        button = 0


def setup():
    global step,button
    size(500,500)
    step = 0 
    button = 0 
    noStroke()


def draw():
    global step
    global button
    background(255)
    if step == 0:
        main_menu()
    elif step == 1:
        game()
    elif step == 2:
        winner()
    elif step == 3:
        loser()
    elif step == 4:
        game2()
    elif step == 5:
        winner2()
    elif step == 6:
        loser2()
    elif step == 7:
        game3()
    elif step == 8:
        winner3()
    elif step ==9:
        loser3()
    elif step == 10:
        game4()
    elif step == 11:
        winner4()
    elif step == 12:
        loser4()
    elif step == 13:
        game5()
    elif step == 14:
        winner5()
    elif step == 15:
        loser5()
  
    else:
        pass

def mouseClicked():
    global button
    if mouseX >= 200 and mouseX <= 300 and mouseY >= 400 and mouseY <= 450:
        button = 1   #main menu/start button
    if mouseX >= 45 and mouseX <= 195 and mouseY >= 410 and mouseY <= 450:
        button = 2    # Answer 1
    elif mouseX >= 300 and mouseX <= 450 and mouseY >= 410 and mouseY <= 450:
        button = 3    # Answer 2
    elif mouseX >= 45 and mouseX <= 195 and mouseY >= 250 and mouseY <= 300:
        button = 4    # Answer 3
    elif mouseX >= 300 and mouseX <= 450 and mouseY >= 250 and mouseY <= 300:
        button = 5    # Answer 4
    elif mouseX >= 40 and mouseX <= 215 and mouseY >= 310 and mouseY <= 360:
        button = 6  #retry button
    elif mouseX >= 290 and mouseX <= 430 and mouseY >= 310 and mouseY <= 360:
        button = 7  #give up button
    elif mouseX >= 180 and mouseX <= 325 and mouseY >= 350 and mouseY <= 400:
        button = 8 #final winner quit button
    else:
        pass
