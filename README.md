# Income-Tax-Calculator
income = int(input())
discounted_income = income - 50000
slab1 = ((5/100)*discounted_income)
slab2 = ((10/100)*discounted_income)
slab3 = ((15/100)*discounted_income)
slab4 = ((20/100)*discounted_income)
slab5 = ((25/100)*discounted_income)
slab6 = ((30/100)*discounted_income)
#Below code would be implemented only if the discounted income lies between 0 and 250000
if (discounted_income > 0) and (discounted_income <= 250000):
    print("Nil")
#Below code would be implemented only if the discounted income lies between 250000 and 500000
if (discounted_income > 250000) and (discounted_income <= 500000):
    print(slab1 - ((5/100)*250000))
#Below code would be implemented only if the discounted income lies between 500000 and 750000
if (discounted_income > 500000) and (discounted_income <= 750000):
    print(slab2 - (((5/100)*250000) + ((10/100)*250000)))
#Below code would be implemented only if the discounted income lies between 750000 and 1000000
if (discounted_income > 750000) and (discounted_income <= 1000000):
    print(slab3 - (((5/100)*250000) + ((10/100)*250000) + ((15/100)*250000)))
#Below code would be implemented only if the discounted income lies between 1000000 and 1250000
if (discounted_income > 1000000) and (discounted_income <= 1250000):
    print(slab4 - (((5/100)*250000) + ((10/100)*250000) + ((15/100)*250000) + ((20/100)*250000)))
#Below code would be implemented only if the discounted income lies between 1250000 and 1500000
if (discounted_income > 1250000) and (discounted_income <= 1500000):
    print(slab5 - (((5/100)*250000) + ((10/100)*250000) + ((15/100)*250000) + ((20/100)*250000) + ((25/100)*250000)))
#Below code would be implemented if the dicoumted income is more than 1500000
if (discounted_income >1500000):
    print(slab6 - (((5/100)*250000) + ((10/100)*250000) + ((15/100)*250000) + ((20/100)*250000) + ((25/100)*250000) + ((30/100)*250000)))
