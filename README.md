# PI-Game-Tic-Tac-Toe-Lily-Chau-Tyler-Watson-
#TIC TAC TOEEEEEEeeeohh you lost. Or did you? Find out if you sit on the Tic Tac Toe Petestal or not in this exclusive game that's FREE #FREE FREE! (-:

from tkinter import *
import tkinter.messagebox
#import Tkinter.messagebox // python 3

tk = Tk()
tk.title("TIC TAC TOE")

click = True

def tictactoe(buttons):
	global click
	if buttons["text"] == " " and click == True:
		buttons["text"] = "X"
		click = False
	elif buttons["text"] == " " and click == False:
		buttons["text"] = "O"
		click = True

	elif(button1["text"] == "X" and button2["text"] == "X" and button3["text"] == "X" or
	     button4["text"] == "X" and button5["text"] == "X" and button6["text"] == "X" or
	     button7["text"] == "X" and button8["text"] == "X" and button9["text"] == "X" or
	     button3["text"] == "X" and button5["text"] == "X" and button7["text"] == "X" or
	     button1["text"] == "X" and button5["text"] == "X" and button9["text"] == "X" or
	     button1["text"] == "X" and button4["text"] == "X" and button7["text"] == "X" or
	     button2["text"] == "X" and button5["text"] == "X" and button8["text"] == "X" or
	     button3["text"] == "X" and button6["text"] == "X" and button9["text"] == "X"):
	     tkinter.messagebox.showinfo("WINNER WINNER CHICKEN DINNER","PLAYER X WON THE GAME")

	elif(button1["text"] == "O" and button2["text"] == "O" and button3["text"] == "O" or
	     button4["text"] == "O" and button5["text"] == "O" and button6["text"] == "O" or
	     button7["text"] == "O" and button8["text"] == "O" and button9["text"] == "O" or
	     button3["text"] == "O" and button5["text"] == "O" and button7["text"] == "O" or
	     button1["text"] == "O" and button5["text"] == "O" and button9["text"] == "O" or
	     button1["text"] == "O" and button4["text"] == "O" and button7["text"] == "O" or
	     button2["text"] == "O" and button5["text"] == "O" and button8["text"] == "O" or
	     button3["text"] == "O" and button6["text"] == "O" and button9["text"] == "O"):
         tkinter.messagebox.showinfo("WINNER WINNER CHICKEN DINNER", "PLAYER O WON THE GAME")


buttons=StringVar()

button1 = Button(tk , text= " ", font=('Times 20 bold'), height= 5, width=9, command=lambda:tictactoe(button1))
button1.grid(row=1, column=0, sticky =S+N+E+W)

button2 = Button(tk , text= " ", font=('Times 20 bold'), height= 5, width=9, command=lambda:tictactoe(button2))
button2.grid(row=1, column=1, sticky =S+N+E+W)

button3 = Button(tk , text= " ", font=('Times 20 bold'), height= 5, width=9, command=lambda:tictactoe(button3))
button3.grid(row=1, column=2, sticky =S+N+E+W)

button4 = Button(tk , text= " ", font=('Times 20 bold'), height= 5, width=9, command=lambda:tictactoe(button4))
button4.grid(row=2, column=0, sticky =S+N+E+W)

button5 = Button(tk , text= " ", font=('Times 20 bold'), height= 5, width=9, command=lambda:tictactoe(button5))
button5.grid(row=2, column=1, sticky =S+N+E+W)

button6 = Button(tk , text= " ", font=('Times 20 bold'), height= 5, width=9, command=lambda:tictactoe(button6))
button6.grid(row=2, column=2, sticky =S+N+E+W)

button7 = Button(tk , text= " ", font=('Times 20 bold'), height= 5, width=9, command=lambda:tictactoe(button7))
button7.grid(row=3, column=0, sticky =S+N+E+W)

button8 = Button(tk , text= " ", font=('Times 20 bold'), height= 5, width=9, command=lambda:tictactoe(button8))
button8.grid(row=3, column=1, sticky =S+N+E+W)

button9 = Button(tk , text= " ", font=('Times 20 bold'), height= 5, width=9, command=lambda:tictactoe(button9))
button9.grid(row=3, column=2, sticky =S+N+E+W)

tk.mainloop()
