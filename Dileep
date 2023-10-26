# Projects
import tkinter as tk

# Function to add a task
def add_task():
    task = task_entry.get()
    if task:
        task_listbox.insert(tk.END, task)
        task_entry.delete(0, tk.END)  # Clear the entry field

# Function to remove a selected task
def remove_task():
    try:
        selected_task_index = task_listbox.curselection()[0]
        task_listbox.delete(selected_task_index)
    except IndexError:
        pass

# Create the main window
root = tk.Tk()
root.title("To-Do List")

# Create a task entry field
task_entry = tk.Entry(root)
task_entry.pack(pady=10)

# Create an "Add Task" button
add_button = tk.Button(root, text="Add Task", command=add_task)
add_button.pack()

# Create a task listbox
task_listbox = tk.Listbox(root)
task_listbox.pack()

# Create a "Remove Task" button
remove_button = tk.Button(root, text="Remove Task", command=remove_task)
remove_button.pack()

# Starting the Tkinter main loop
root.mainloop()
