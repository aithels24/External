# External
#Write
#This section writes thing in the file and starts it 
hname = input("Whats the horse name?")

file = open('char.txt', 'w')
file.write("Your charater is a horse")
file.write("\n Its name is \n")
file.write(hname + ',')

file.close()

#This part lets me add things in when the file first closed
print("\n We forgot the last name")

def append():
    lastname = input("Whats its last name?")

    file = open('char.txt', 'a')
    file.write('\n last name is \n')
    file.write(lastname + ',')
    
    file.write('\n full name\n')
    file.write(hname +  lastname)

    file.close()

#read
    
append()

look = open("char.txt", "r")
print(look.read())
