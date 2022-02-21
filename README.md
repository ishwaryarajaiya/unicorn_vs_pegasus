# unicorn_vs_pegasus
a simple game
def unicorn_vs_pegasus():
    select=input("type unicorn or pegasus")
    if select=='unicorn':
        print("you have selected Unicorn")
        return("unicorn")
    elif select=='pegasus':
        print("you have selected Pegasus")
        return("pegasus")
unicorn_vs_pegasus()

import random
dice=random.randint(1,8)

points=0
while(points<9):
 while(dice>1):
    print("You have not collected the body.")
    print("TRY AGAIN!!!")
    dice = random.randint(1,8)
    print("DICE=", dice)
    
 if(dice==1):
    print("BODY COLLECTED")
    points=points+1
    print("point=",points)
    print("now roll the dice again to continue the game")
    pass
    dice = random.randint(1,8)
    print("dice=",dice)
    
    
 upper_part= {2:'tail',3:'leg',7:'wing'}

 if(dice in upper_part.keys()):
  val=upper_part[dice]
  points=points+1
  print('you rolled',dice,'COLLECTED',val)
  print("points=",points)
  
  if(dice==5,6,8):
      print("you have to collect head first")
      dice=random.randint(1,8)
   
  if(dice==4):
    print("HEAD COLLECTED")
    points=points+1
    print("point=",points)
    print("now roll the dice again to continue the game")
    pass
    dice = random.randint(1,8)
    print("dice=",dice)
    
    face_part= {5:'eye',6:'mouth',8:'horn'}

    if(dice in face_part.keys()):
      val=face_part[dice]
      points=points+1
      print('you rolled',dice,'COLLECTED',val)
      print("points=",points)
