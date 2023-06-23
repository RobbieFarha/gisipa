import tkinter as tk
from tkinter import font
import random

def database_extracting_tool():
    num1 = random.randint(2, 128)
    num2 = random.randint(2, 128)
    operator = random.choice(['+', '-'])
    problem = f"What is {num1} {operator} {num2}?"

    label.config(text=problem)

    entry.delete(0, tk.END)
    check_button.config(command=lambda: check_answer(entry.get(), num1, num2, operator))

def check_answer(answer, num1, num2, operator):
    try:
        user_answer = int(answer)
        if operator == '+':
            correct_answer = num1 + num2
        elif operator == '-':
            correct_answer = num1 - num2

        if user_answer == correct_answer:
            result = "Correct!"
        else:
            result = f"Incorrect. The correct answer is {correct_answer}."
    except ValueError:
        result = "Invalid input. Please enter a number."

    result_label.config(text=result)

def option2():
    print("Option 2 selected.")

def option3():
    print("Option 3 selected.")

def option4():
    print("Option 4 selected.")

def option5():
    print("Option 5 selected.")

def option6():
    print("Option 6 selected.")

def file_explorer():
    print("File Explorer selected.")

def system_preferences():
    print("System Preferences selected.")

def logoff():
    print("LOGOFF selected.")

def main_menu():
    window = tk.Tk()
    window.title("GISIPA Network")  # Update the title of the window
    window.configure(bg="black")

    # Adjust window size
    window.geometry("400x400")

    # Define font styles
    heading_font = font.Font(family="VCR OSD MONO", size=72)
    body_font = font.Font(family="VCR OSD MONO", size=28)

    label = tk.Label(window, text="GISIPA Network", fg="white", bg="black", font=heading_font)
    label.pack(pady=10)

    button1 = tk.Button(window, text="Database Extracting Tool", command=database_extracting_tool, bg="black", fg="white", font=body_font)
    button1.pack()

    button2 = tk.Button(window, text="Option 2", command=option2, bg="black", fg="white", font=body_font)
    button2.pack()

    button3 = tk.Button(window, text="Option 3", command=option3, bg="black", fg="white", font=body_font)
    button3.pack()

    button4 = tk.Button(window, text="Option 4", command=option4, bg="black", fg="white", font=body_font)
    button4.pack()

    button5 = tk.Button(window, text="Option 5", command=option5, bg="black", fg="white", font=body_font)
    button5.pack()

    button6 = tk.Button(window, text="Option 6", command=option6, bg="black", fg="white", font=body_font)
    button6.pack()

    result_label = tk.Label(window, text="", fg="white", bg="black", font=body_font)
    result_label.pack(pady=10)

    entry = tk.Entry(window, font=body_font, width=10)
    entry.pack(pady=10)

    check_button = tk.Button(window, text="Check Answer", command=None, bg="black", fg="white", font=body_font)
    check_button.pack(pady=10)

    exit_button = tk.Button(window, text="LOGOFF", command=logoff, bg="black", fg="white", font=body_font)
    exit_button.pack(pady=20)

    window.mainloop()

# Run the main menu
main_menu()
