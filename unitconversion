import tkinter as tk
from tkinter import ttk

def cm_to_feet():
    try:
        cm = float(cm_entry.get())
        feet = cm * 0.0328084
        result_label.config(text=f"{cm} centimeters = {feet:.2f} feet")
    except ValueError:
        result_label.config(text="Please enter a valid number")

def feet_to_inches():
    try:
        feet = float(feet_entry.get())
        inches = feet * 12
        result_label.config(text=f"{feet} feet = {inches:.2f} inches")
    except ValueError:
        result_label.config(text="Please enter a valid number")

def sqft_to_sqm():
    try:
        sqft = float(sqft_entry.get())
        sqm = sqft * 0.092903
        result_label.config(text=f"{sqft} sqft = {sqm:.2f} sqm")
    except ValueError:
        result_label.config(text="Please enter a valid number")

def sqft_to_hectares_acres():
    try:
        sqft = float(sqft_to_hectares_acres_entry.get())
        hectares = sqft * 0.0000092903
        acres = sqft * 0.0000229568
        result_label.config(text=f"{sqft} sqft = {hectares:.6f} hectares\n{sqft} sqft = {acres:.6f} acres")
    except ValueError:
        result_label.config(text="Please enter a valid number")

# Create main window
root = tk.Tk()
root.title("Unit Converter")
root.geometry("450x270")
root.configure(background='#f0f0f0')

# Create style for buttons
style = ttk.Style()
style.configure('TButton', background='#4caf50', foreground='#000000', font=('Arial', 10, 'bold'))

# Create centimeter to feet conversion widgets
cm_label = tk.Label(root, text="Centimeters:", background='#f0f0f0', font=('Arial', 12))
cm_label.grid(row=0, column=0, padx=10, pady=10, sticky='w')
cm_entry = tk.Entry(root)
cm_entry.grid(row=0, column=1, padx=10, pady=10)
cm_to_feet_button = ttk.Button(root, text="Convert to Feet", command=cm_to_feet)
cm_to_feet_button.grid(row=0, column=2, padx=10, pady=10)

# Create feet to inches conversion widgets
feet_label = tk.Label(root, text="Feet:", background='#f0f0f0', font=('Arial', 12))
feet_label.grid(row=1, column=0, padx=10, pady=10, sticky='w')
feet_entry = tk.Entry(root)
feet_entry.grid(row=1, column=1, padx=10, pady=10)
feet_to_inches_button = ttk.Button(root, text="Convert to Inches", command=feet_to_inches)
feet_to_inches_button.grid(row=1, column=2, padx=10, pady=10)

# Create square feet to square meters conversion widgets
sqft_label = tk.Label(root, text="Square Feet:", background='#f0f0f0', font=('Arial', 12))
sqft_label.grid(row=2, column=0, padx=10, pady=10, sticky='w')
sqft_entry = tk.Entry(root)
sqft_entry.grid(row=2, column=1, padx=10, pady=10)
sqft_to_sqm_button = ttk.Button(root, text="Convert to Sqm", command=sqft_to_sqm)
sqft_to_sqm_button.grid(row=2, column=2, padx=10, pady=10)

# Create square feet to hectares/acres conversion widgets
sqft_to_hectares_acres_label = tk.Label(root, text="Square Feet:", background='#f0f0f0', font=('Arial', 12))
sqft_to_hectares_acres_label.grid(row=3, column=0, padx=10, pady=10, sticky='w')
sqft_to_hectares_acres_entry = tk.Entry(root)
sqft_to_hectares_acres_entry.grid(row=3, column=1, padx=10, pady=10)
sqft_to_hectares_acres_button = ttk.Button(root, text="Convert to Hectares/Acres", command=sqft_to_hectares_acres)
sqft_to_hectares_acres_button.grid(row=3, column=2, padx=10, pady=10)

# Result frame
result_frame = tk.LabelFrame(root, text="Result", background='#f0f0f0', font=('Arial', 12))
result_frame.grid(row=4, column=0, columnspan=3, padx=10, pady=10)
result_label = tk.Label(result_frame, text="", background='#f0f0f0', font=('Arial', 12))
result_label.pack()

root.mainloop()
