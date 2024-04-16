#atm-code
import datetime
sediment=[]
extract=[]
balance=0
while True:
   
    Atm =    input("1:balance\n2:Deposite\n3:widthrawal\n4:transaction_history\n")
    if Atm == '1':
    
        print(balance, "is your ballance")
        

    elif Atm=='2':
        deposite=int(input("enter amount"))
        balance=deposite + balance 
        sediment.append(deposite,)
        
        print(balance,"deposite was succesful")
       
    elif Atm=='3':
        widthrawal= int (input("amount"))
        if widthrawal> balance:
            print("insufficient funds")
        elif widthrawal< balance:
            balance=balance - widthrawal
            extract.append(widthrawal,)
            print(widthrawal,"widthrawal was succesful")
    elif Atm=='4':
        #  transaction_history=sediment + extract
         print(sediment , extract, )
            



