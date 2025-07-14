# Iner Planetary Weights Calculator

# 1. Surface Gravity Factors
nMercurySGF = 0.38
nVenusSGF = 0.91
nMoonSGF = 0.165
nMarsSGF = 0.38
nJupiterSGF = 2.34
nSaturnSGF = 0.93
nUranusSGF = 0.92
nNeptuneSGF = 1.12
nPlutoSGF = 0.066

# 2. Input Name and Weight
sName = input ("Enter your name: ")
nWeight = float(input("Enter your weight on Earth: "))

# 3. Calculate Weight on Planets
print(sName,"here are your weights on our Solar System's planets:")

nMercurySGF *= nWeight
print("{:<20} {:>10,.2f}".format("Weight on Mercury:", nMercurySGF))

nVenusSGF *= nWeight
print("{:<20} {:>10,.2f}".format("Weight on Venus:", nVenusSGF))

nMoonSGF *= nWeight
print("{:<20} {:>10,.2f}".format("Weight on Moon:", nMoonSGF))

nMarsSGF *= nWeight
print("{:<20} {:>10,.2f}".format("Weight on Mars:", nMarsSGF))

nJupiterSGF *= nWeight
print("{:<20} {:>10,.2f}".format("Weight on Jupiter:", nJupiterSGF))

nSaturnSGF *= nWeight
print("{:<20} {:>10,.2f}".format("Weight on Saturn:", nSaturnSGF))

nUranusSGF *= nWeight
print("{:<20} {:>10,.2f}".format("Weight on Uranus:", nUranusSGF))

nNeptuneSGF *= nWeight
print("{:<20} {:>10,.2f}".format("Weight on Neptune:", nNeptuneSGF))

nPlutoSGF *= nWeight
print("{:<20} {:>10,.2f}".format("Weight on Pluto:", nPlutoSGF))
