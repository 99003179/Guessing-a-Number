import random


class guess:
    def __init__(self):
        print("Enter a number between 1 and 100")
        self.num = input()

    class personaldetails:
        def __init__(self):
            print("enter your name")
            self.name = input()

        def print(self):
            print ("your name is ", self.name)

    def guess1(self):
        random_number = random.randint(1, 100)
        win = False
        Turns = 0
        while win == 0:
            Turns += 1
            if random_number == int(self.num):
                print("You won!")
                print("Number of turns you have used: ", Turns)
                win == 1
                break
            else:
                if random_number > int(self.num):
                    print("Your Guess was low, Please enter a higher number")
                else:
                    print("your guess was high, please enter a lower number")
obj1 = guess.personaldetails()
obj1.print()
obj = guess()
obj.guess1()
