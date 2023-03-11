# DZ4
class Rex():
 print("Raaar")
 def __init__(self,height,age):
 self.height = height
 self.age = age
 print(f"I am alive and i am {self.height} size and {age} years old! Rar")
 def question(self):
 print('may i ask question?')
first_student = Rex(340,16)


class Rex:
 def __init__(self, height):
 self.height = height
 print(f"I am alive and i am {self.height} size")
Raks = Rex(360)
Rexi = Rex(350)
print(Raks)
print(Rexi)

class Rex:
 amount_of_students = 0
 def __init__(self, height=160):
 self.height = height
 Rex.amount_of_students += 1
Raks = Rex ()
Rexi = Rex(height=360)
print(Raks.amount_of_students)
print(Rexi.amount_of_students)



class Rex:
 height = 360
 def __init__(self):
 print(self.height)
 self.height+=10
Raks = Rex()
Rexi = Rex()



class Rex:
 def __init__(self):
 self.height = 370
 height = 360
 def printer(self):
 print(self.height)
Reks = Rex()
Reks.printer()


#Methods
#grow() - change size of the student
class Rex:
 amount_of_students = 0
 def __init__(self, height=360):
 self.height = height
 Rex.amount_of_students += 1
 print(self.amount_of_students)
 print(self.height)
 def grow(self, height = 1):
 self.height += height
 return self.height
Reks = Rex()
Rexi = Rex(height=370)
print(Reks.grow())


#__str__() -Чтобы во время выведения объекта не получать строку с непонятным содержимым
class Rex:
 def __init__(self, name=None):
 self.name = name
 def __str__(self):
 return f"I am a Rex. My name is {self.name}."
Reks = Rex(name="Reks")
print(Reks.__str__())

#__del__() - Метод позволяющий удалить объект

class Rex:
 def __init__(self, name=None):
 self.name = name
 def __del__(self):
 print("Training is over.I am now an expert!")
Reks = Rex()




import random
class Student:
 def __init__(self, Rex):
 self.Rex = Rex
 self.gladness = 50
 self.progress = 0
 self.hungry = 0
 self.alive = True
 def to_study(self):
 print("Time to eat")
 self.progress += 0.12
 self.gladness -= 5
 self.hungry -= 100
 def to_sleep(self):
 print("I will sleep")
 self.gladness += 3

 def hung(self):
 self.hungry += 10
 return self.hungry

 def to_chill(self):
 print("Rest time")
 self.gladness += 5
 self.progress -= 0.1
 self.money()

 def is_alive(self):
 if self.progress < -0.5:
 print("Cast out…")
 self.alive = False
 elif self.gladness <= 0:
 print("Depression…")
 self.alive = False
 elif self.progress > 5:
 print("Passed externally…")
 self.alive = False
 elif self.hungry < 20:
 print("Passed externally…")
 self.alive = False

 def end_of_day(self):
 print(f"Gladness = {self.gladness}")
 print(f"Progress ={round(self.progress, 2)}")

 def live(self, day):
 day = "Day" + str(day) + "of" + self.name + "life"
 print(f"{day:=^50}")
 if self.money < 100:
 self.work()
 live_cube = random.randint(1, 3)
 if live_cube == 1:
 self.to_study()
 elif live_cube == 2:
 self.to_sleep()
 elif live_cube == 3:
 self.to_chill()
 self.end_of_day()
 self.is_alive()

Reks = Rex(name="Reks")
for day in range(365):
 if Reks.alive == False:
 break
 Rex.live(day)
 print(day)
 
