playing = True
first_time = True

#play again function
def play_again():
  global playing
  global first_time
  while True:
    play_again_input = input("Do you want to play again? (Enter Y or N) ")
    if play_again_input.upper() == 'Y' or play_again_input.upper() == 'N':
      break
    else:
      print("That was not a valid input. Please answer with either Y or N.")
  if play_again_input.upper() == 'N':
    playing = False
  else: 
    first_time = False
#actual game code
while playing:
  print('''
######## ####  #######  ##    ## 
     ##   ##  ##     ## ###   ## 
    ##    ##  ##     ## ####  ## 
   ##     ##  ##     ## ## ## ## 
  ##      ##  ##     ## ##  #### 
 ##       ##  ##     ## ##   ### 
######## ####  #######  ##    ##

''')
  #asks for name and if player wants to play
  if first_time == True:
    name = input("Hi! What is your name? ")

    while True:
      player_input = input(f"Hello {name}, do you want to play? (Enter Y for Yes or N for No) ")
      if player_input.upper() == 'Y' or player_input.upper() == 'N':
        break
      else:
        print("That was not a valid input. Please answer with either Y or N.")
    if player_input.upper() == 'N':
      break

    #beginning of game
    print('''
Welcome to Zion. 
You’re part of a team of scientists, detectives, engineers, etc. from Psych Inc. who are trying to destroy a harmful serum that could potentially annihilate the planet. 
The serum is made by an evil corporation called Zion. It is up to you to steal the serum and escape from Eve Il, the head of Zion. 
Good luck!\n''')

  else:
    print("Welcome back!\n")

  #prompt1
  while True:
    prompt1 = input('''You’ve reached the base of Zion’s towering building and now you have to find a way in. Will you… (choose between A and B)

A. Nab an exiting Zion employee and steal their ID badge to enter the building normally through the front door as if you aren’t trying to take a world-destructive serum.

B. Climb the building walls using your untrustworthy climbing gear and enter the room in which the serum is stored through the roof.

''')
    if prompt1.upper() == 'A' or prompt1.upper() == 'B':
      break
    else:
      print("\nThat was not a valid input. Please answer with either A or B.")
  if prompt1.upper() == 'A':
    print("\nYou have successfully gotten in.\n")
    #prompt2
    while True:
      try:
        prompt2 = int(input('''Choose Door 1 or Door 2 (type 1 or 2). 
Only one leads to the serum, and the other one leads to a room which triggers an intruder alarm, in which case you lose.\n
'''))
      except ValueError:
        print('\nThat is not a valid input. Try again.\n')
        continue
      if prompt2 == 1 or prompt2 == 2:
        break
      else:
        print("\nThat was not a valid input. Please answer with either 1 or 2.")
    if prompt2 == 1: 
      print('''\nSorry, you have triggered the intruder alarm. 

   
  / ____|   /\   |  \/  |  ____|  / __ \ \    / /  ____|  __ \  |
 | |  __   /  \  | \  / | |__    | |  | \ \  / /| |__  | |__) | |
 | | |_ | / /\ \ | |\/| |  __|   | |  | |\ \/ / |  __| |  _  /  |
 | |__| |/ ____ \| |  | | |____  | |__| | \  /  | |____| | \ \  |
  \_____/_/    \_\_|  |_|______|  \____/   \/   |______|_|  \_\ *
                                                               
The Zion guards caught you and imprisoned you. Game over!''')
      play_again()
      continue
    else:
      print ("\nGood job! You snuck into the right room and are currently standing behind an oblivious Dr. Eve Il. ")
      #prompt3
      while True:
        prompt3 = input('''\n Will you... (choose A or B)
A. Go up and grab the serum, and then run for all you're worth out of the building
      
B. Be extremely stealthy and sneak up and steal the serum when Eve Il isn't looking, then normally walk out of the building, sporting your "badge" \n\n''')
        if prompt3.upper() == 'A' or prompt3.upper() == 'B':
          break
        else:
          print("\nThat was not a valid input. Please answer with either A or B.\n")
      if prompt3.upper() == 'A':
        print ('''Sorry, game over -- obviously Eve Il has secret Ilbots that can penetrate the floor in the case of an emergency, so they caught you and imprisoned you in the Level 14 dungeon. Good luck next time!
        
      / ____|   /\   |  \/  |  ____|  / __ \ \    / /  ____|  __ \  |
     | |  __   /  \  | \  / | |__    | |  | \ \  / /| |__  | |__) | |
     | | |_ | / /\ \ | |\/| |  __|   | |  | |\ \/ / |  __| |  _  /  |
     | |__| |/ ____ \| |  | | |____  | |__| | \  /  | |____| | \ \  |
      \_____/_/    \_\_|  |_|______|  \____/   \/   |______|_|  \_\ *
                                                               ''')
        play_again()
        continue
      elif prompt3.upper() == "B":
        print("\nGood choice! Eve Il didn't catch you and you were able to escape. Onto your next mission: \n")
      
  else:
    print ('''\nYour rope was cheap quality and broke! You broke your ankle and you're going to have to postpone your mission. 
    
  / ____|   /\   |  \/  |  ____|  / __ \ \    / /  ____|  __ \  |
 | |  __   /  \  | \  / | |__    | |  | \ \  / /| |__  | |__) | |
 | | |_ | / /\ \ | |\/| |  __|   | |  | |\ \/ / |  __| |  _  /  |
 | |__| |/ ____ \| |  | | |____  | |__| | \  /  | |____| | \ \  |
  \_____/_/    \_\_|  |_|______|  \____/   \/   |______|_|  \_\ *

                                                               ''')
    play_again()
    continue
  
  print("Great job stealing the serum, but you were a hair away from being caught. You are currently on the run from Eve Il (who discovered the serum was missing), and you must reach the next town, which is 100 miles away (at which point you're confident that she will give up), and find a way to obliterate it. You will have to make choices about what you will do to make it safely. You can make money along the way, which you can use to replenish your health. You'll lose if your health drops to zero, or if Eve Il catches up to you. Good luck!\n")

  user_distance = 150
  evil_distance = 160
  health = 10
  money = 0
  job = False
  
  while True:
    while True:
      distance_behind = evil_distance - user_distance
      user_prompt = input(f'''
1. Walk at a moderate speed
2. Walk at a brisk speed
3. Run for your life (mind you, this will get you tired)
4. Get a temporary job and make a little money
5. Quit your job
6. Buy food and water (which costs $3)
7. Quit
YOUR MONEY: {money}
YOUR HEALTH: {health}
You are {user_distance} miles away from the town.
Eve Il is {distance_behind} miles behind you. \n
''' )
      if user_prompt == "1" or user_prompt == "2" or user_prompt == "3" or user_prompt == "4" or user_prompt == "5" or user_prompt == "6" or user_prompt == "7":
        break
      else:
        print("\nThat was not a valid input. Please answer with 1, 2, 3, 4, 5, 6, or 7.")

    if (user_prompt == "1"):
      user_distance -= 5
      evil_distance -= 4
      health -= 0.2

    elif (user_prompt == "2"): 
     user_distance -= 6
     evil_distance -= 4
     health -= 0.4

    elif (user_prompt == "3"): 
     user_distance -= 8
     evil_distance -= 4
     health -= 1

    elif (user_prompt == "4"): 
      evil_distance -= 4
      if job == False: 
       job = True
       money += 5
       health -= 0.1
       print (f"\nYou now have a job. Your money is ${money}")
      else: 
        print ("\nYou already have a job.")
        health -= 0.1
        money += 5

    elif (user_prompt == "5"): 
      if job == True: 
       job = False
       print ("\nYou have now quit your job.")
      else: 
       print ("\nYou don't have a job yet.")

    elif user_prompt == "6": 
      if money >= 3:
        money -= 3
        evil_distance -= 4
        health += 3
      else:
        print("\nSorry, you don't have enough money.\n")

    elif user_prompt == "7": 
      print ("\nThanks for making an attempt to save humanity from Zion. We hope to see you back soon!\n")
      break

    if health <= 0:
      print("\nThank you for trying, but your health has reached 0. You collapsed from hunger and thirst.\n")
      break

    if health < 3: 
      print("\nYou are getting tired! You should get food and water.\n")

    if distance_behind <= 0:
      print("\nSorry! You lost. Eve Il has caught up to you. She's taking you and the serum back to Zion Corp. where she will take back the serum and lock you away in the level 14 dungeon and unleash her deadly komodo dragon Chaos on you. Thanks for trying!\n")
      break
    
    if user_distance <= 0: 
      print('''\nYOU HAVE WON! You reached the next town and Eve Il has given up trying to chase you. You were able to safely destroy the serum (by chucking it into a multi-acre landfill). Thanks for playing!\n''')
      break
  play_again()
  
