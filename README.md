# searchbar from tkinter import *
import webbrowser
t=Tk()
t.geometry("400x400")
def send():
    g=inputt.get()
    d=webbrowser.open("www.{}.com".format(g))
Label(t,text="Mysearch",font="arial 26 bold").pack(padx=5,pady=5)
inputt=Entry(t,width=60,borderwidth=0,font="arial 26 bold")
inputt.pack(padx=5,pady=5)
inputt.insert('end','Search here')
btn=Button(t,text="Search",font="arial 26 bold",command=send)
btn.pack(padx=5,pady=5)
t.mainloop()
