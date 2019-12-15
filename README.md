# Paint-Job-Function
# PART 1
# Keep user in a loop until a valid number is entered
def getFloatInput(value, minimum):
    while True:
        number = True  # as long as number is not true the loop will keep happening
        userinput = input(value)
        for letter in userinput:  # the for loop check every single letter inside a variable
            if letter.isalpha():  # if the variable contains a letter then loop again
                number = False
        if number:
            if float(userinput) < minimum:  # Check if the variable did not meet the requirement for a minimum number
                print('You enter a number less than {}. Please enter a greater number'.format(minimum))
            else:
                return float(userinput)
        else:
            print("Please, enter a positive number")


# Return the amount of gallons needed to finish the paint
def getGallonsOfPaint():
    print('Gallons of paint')


# Return the amount of hours it takes for the labor
def getLaborHours():
    print('Hours of Labor')


# Return the total cost of the full labor
def getLaborCost():
    print('Labor cost')


# Return the total cost of the wall paint
def getPaintCost():
    print('Paint charges')


# Return the correct tax sale depending the state chosen
def getSalesTax():
    print('Sale Tax')


# Return the correct tax sale depending the state chosen
def showCostEstimate():
    print('Cost estimate')


# PART 2
# Define output
fWallPrice = getFloatInput('Enter wall space in square feet: ', 0)
fQuareFeet = getFloatInput("Enter paint price per gallon: ", 1)
fPaintPrice = getFloatInput("Enter feet per gallon: ", 1)
fLaborHours = getFloatInput("How many labor hours per gallon: ", 1)
fLaborCost = getFloatInput("Labor charge per hour: ", 1)
sState = input("State job is in: ")


getGallonsOfPaint()
getLaborHours()
getLaborCost()
getPaintCost()
getSalesTax()
showCostEstimate()

# fGallonsPaint = getFloatInput("Enter gallons of Paint:",0);
# fHoursLabor =getFloatInput("Hours of Labor:",0);

        

