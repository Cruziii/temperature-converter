

[# temperature_converter.py](https://github.com/user-attachments/files/24801417/temperature_converter.py)
# temperature_converter.py
def celsius_to_fahrenheit(c): return (c * 9/5) + 32
def fahrenheit_to_celsius(f): return (f - 32) * 5/9

print("Temperature Converter")
while True:
    choice = input("\n1. Celsius to Fahrenheit\n2. Fahrenheit to Celsius\n3. Exit\nChoice: ")
    if choice == '1': 
        c = float(input("Enter Celsius: "))
        print(f"{c}°C = {celsius_to_fahrenheit(c):.1f}°F")
    elif choice == '2':
        f = float(input("Enter Fahrenheit: "))
        print(f"{f}°F = {fahrenheit_to_celsius(f):.1f}°C")
    elif choice == '3': 
        print("Goodbye!"); break
    else: print("Invalid choice. Try again.")
