# Assignment-8
# To determine alkalinity of given sample
H2S04_reg = float(input("Enter the volume of H2S04 required in ml:"))
Sample = float(input("Enter the value of sample in litres:"))
Alkalinity_Removed = H2S04_reg
print("Alkalinity Removed: ", Alkalinity_Removed, "'mg")
Alk_mgperlit = Alkalinity_Removed / Sample
print("Total Alkalinity:", Alk_mgperlit, "mg/lit")
OH= float (input("Enter the value of OH-Alkalinity present : "))
#Alkalinity removed till pH of 8.3
H2S04_req = float (input("Enter the volume of H2S04 required in ml :"))
Alkalinity_Removed = H2S04_req
print("Alkalinity Removed: ",Alkalinity_Removed, "mg")
CO3_Combined = Alkalinity_Removed/Sample
print ("Carbonate Alkalinity upto pH8.3:",CO3_Combined, "mgperlit" )
CO3 = CO3_Combined - OH
print("Carbonate Alkalinity:", CO3,"'mg/lit")
HCO3 = Alk_mgperlit - 2*CO3 - OH
print("Bicarbonate Alkalinity:", HCO3, "mg/it")
