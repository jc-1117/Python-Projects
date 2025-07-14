# 1. Welcome message
print("Welcome to Jacelyn's Temperature Converter!")

# 2. Prompt for temperature
flt_temp = float(input("Enter the temperature: "))

# 3. Promt for temperature scale
str_scale = input("Is the temp F for Farenheit or C for Celsius?: ").lower()

# 4. Check if scale is valid
if str_scale != 'f' and str_scale != 'c':
  print("You must enter a F or C")
else:
  if str_scale == 'f':
    if flt_temp > 212:
      print("Temp can not be > 212")
    else: 
      flt_celsius = (5.0 / 9.0) * (flt_temp - 32)
      print(f"The Celsius equivalent is: {flt_celsius:.1f}")
  else: # str_scale == 'c'
    if flt_temp > 100:
      print("Temp can not be > 100")
    else:
      flt_fahrenheit = (9.0 / 5.0) * flt_temp + 32
      print(f"The Fahrenheit equivalent is: {flt_fahrenheit:.1f}")
