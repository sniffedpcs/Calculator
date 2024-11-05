# import tKinter
from tkinter import *

calWindow = Tk()
calWindow.title('Calculator')
calWindow.geometry('515x365')
calWindow.resizable(0,0)

# Functions: Equal Button Function
def btn_Equal():
    global expression
    results = str(eval(expression))
    input_text.set(results)
    expression = ""

# Functions: Clear Input Function
def btn_Clear():
    global expression
    expression = ""
    input_text.set("")

# Functions: Button Click Function
def btnClick(item):
    global expression
    expression = expression + str(item)
    input_text.set(expression)

# Create Varaible to hold entry
expression = ""
input_text = StringVar()

# Input Frame 
input_frame = Frame(calWindow, width = 312, height = 50)
input_frame.pack(side = TOP)

# Insert Input field into the 'Frame'
input_field = Entry(input_frame, font=('arial', 18, 'bold'), width = 45, justify = RIGHT, textvariable = input_text)
input_field.grid(row=0, column=0)

#increase the size of the input field
input_field.pack(ipady=10)

#Create Button frame
btn_frame = Frame(calWindow, width=310, height=270)
btn_frame.pack()

# Create First Row Buttons
clear  = Button(btn_frame, text = "C", width = 38, height = 3, command=lambda: btn_Clear()).grid(row = 0, column = 0, columnspan = 3, padx = 1, pady = 1)
divide = Button(btn_frame, text = "/", width = 10, height = 3, command=lambda: btnClick('/')).grid(row = 0, column = 3, padx = 1, pady = 1)

# Create Second Row Buttons
seven    = Button(btn_frame, text = "7", width = 10, height = 3, command=lambda: btnClick(7)).grid(row = 1, column = 0, padx = 1, pady = 1)
eight    = Button(btn_frame, text = "8", width = 10, height = 3, command=lambda: btnClick(8)).grid(row = 1, column = 1, padx = 1, pady = 1)
nine     = Button(btn_frame, text = "9", width = 10, height = 3, command=lambda: btnClick(9)).grid(row = 1, column = 2, padx = 1, pady = 1)
multiply = Button(btn_frame, text = "*", width = 10, height = 3, command=lambda: btnClick('*')).grid(row = 1, column = 3, padx = 1, pady = 1)

# Create Third Row Buttons
four  = Button(btn_frame, text = "4", width = 10, height = 3, command=lambda: btnClick(4)).grid(row = 2, column = 0, padx = 1, pady = 1)
five  = Button(btn_frame, text = "5", width = 10, height = 3, command=lambda: btnClick(5)).grid(row = 2, column = 1, padx = 1, pady = 1)
six   = Button(btn_frame, text = "6", width = 10, height = 3, command=lambda: btnClick(6)).grid(row = 2, column = 2, padx = 1, pady = 1)
minus = Button(btn_frame, text = "-", width = 10, height = 3, command=lambda: btnClick('-')).grid(row = 2, column = 3, padx = 1, pady = 1)

# Create Fourth Row Buttons 
one   = Button(btn_frame, text = "1", width = 10, height = 3, command=lambda: btnClick(1)).grid(row = 3, column = 0, padx = 1, pady = 1)
two   = Button(btn_frame, text = "2", width = 10, height = 3, command=lambda: btnClick(2)).grid(row = 3, column = 1, padx = 1, pady = 1)
three = Button(btn_frame, text = "3", width = 10, height = 3, command=lambda: btnClick(3)).grid(row = 3, column = 2, padx = 1, pady = 1)
plus  = Button(btn_frame, text = "+", width = 10, height = 3, command=lambda: btnClick('+')).grid(row = 3, column = 3, padx = 1, pady = 1)

# Create Fifth Row Buttons
zero   = Button(btn_frame, text = "0", width = 24, height = 3, command=lambda: btnClick(0)).grid(row = 4, column = 0, columnspan = 2, padx = 1, pady = 1)
point  = Button(btn_frame, text = ".", width = 10, height = 3, command=lambda: btnClick('.')).grid(row = 4, column = 2, padx = 1, pady = 1)
equals = Button(btn_frame, text = "=", width = 10, height = 3, command=lambda: btn_Equal()).grid(row = 4, column = 3, padx = 1, pady = 1)

calWindow.mainloop()
