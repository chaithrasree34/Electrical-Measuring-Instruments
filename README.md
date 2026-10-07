# Electrical-Measuring-Instruments
# Electrical Measuring Instruments
# Python Program

print("====================================")
print(" ELECTRICAL MEASURING INSTRUMENTS")
print("====================================")

print("\n1. Voltmeter - Measures Voltage")
print("2. Ammeter - Measures Current")
print("3. Wattmeter - Measures Power")
print("4. Energy Meter - Measures Electrical Energy")

choice = int(input("\nEnter your choice (1-4): "))

if choice == 1:
    current = float(input("Enter current in Amperes: "))
    resistance = float(input("Enter resistance in Ohms: "))
    voltage = current * resistance
    print("Voltage =", voltage, "V")

elif choice == 2:
    voltage = float(input("Enter voltage in Volts: "))
    resistance = float(input("Enter resistance in Ohms: "))
    current = voltage / resistance
    print("Current =", current, "A")

elif choice == 3:
    voltage = float(input("Enter voltage in Volts: "))
    current = float(input("Enter current in Amperes: "))
    power_factor = float(input("Enter power factor: "))
    power = voltage * current * power_factor
    print("Power =", power, "W")

elif choice == 4:
    power = float(input("Enter power in Watts: "))
    time = float(input("Enter operating time in hours: "))
    energy = (power * time) / 1000
    print("Electrical Energy =", energy, "kWh")

else:
    print("Invalid choice!")

print("\nProgram completed successfully