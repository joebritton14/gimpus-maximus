# gimpus-maximus
def salesLoop():
    absTotal = 0
    totalVat = 0
    vat = 0
    figList = []
    afterVatList = []
    while True:
        figNum = input("Enter a sales figure <Enter -1 to finish>: ")
        figList.append(int(figNum))
        if figNum == "-1":
            break

    del figList[-1]
    print("The sales figures entered were: " , figList)

    for n in figList:
        vat = n * 0.23
        totalVat += vat
        n = n + vat
        absTotal += n
        afterVatList.append(n)

    print("The sales figures after VAT are: " , afterVatList)
    print("The total Vat is: " , totalVat)
    print("The total sales for this period are: ", absTotal)
