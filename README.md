# Tkinter-tips-and-tricks
Here we have used some more features and tricks present in Tkinter
Code:



from tkinter import *
root = Tk()
root.geometry("655x452")
root.title("Tips and Tricks")

root.wm_iconbitmap("1.ico")     #To change the icon before the title   wm.iconbitmap("image_filename")   is used

root.config(background="orange")        #Sets the background color. You can also write "bg"
Label(root, text="Hii there!", bg="lightblue", fg="red").pack(fill=X, pady=30, ipady=20)    #"ipady or ipadx provides internal spacing"
Button(root, text="Close", command=root.destroy, bg="grey", relief=FLAT).pack(pady=20)    #"root.destroy is an internal command and hence need not to be defined"

width = root.winfo_screenwidth()    #Tells the width of your monitor screen
height = root.winfo_screenheight()  #Tells the height of your monitor screen
print(f"The width and height of the window is {width} x {height}")
root.mainloop()
