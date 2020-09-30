from time import sleep

while True:
    choice = input("Menu:\n1.insert number\n2.please insert 4 IPs\n3.please insert a 4 DNS\n4.palindrome\n")
    if choice == "1":
        print("\nthe new number is: \n" + str((int(input("please enter a number: "))) ** 3))
    elif choice == "2":
        list_ip = [input("enter new ip"), input("enter new ip"), input("enter new ip"), input("enter new ip")]
        sleep(3)
        print("the new list: " + str(list_ip))
    elif choice == "3":
        dns_dict = {}
        dns_dict.update({input("Enter a URL: "): input("Enter IP: ")})
        dns_dict.update({input("Enter a URL: "): input("Enter IP: ")})
        dns_dict.update({input("Enter a URL: "): input("Enter IP: ")})
        dns_dict.update({input("Enter a URL: "): input("Enter IP: ")})
        sleep(3)
        print("the new dns_dict: \n" + str(dns_dict))
    elif choice == "4":
        word = input("enter a word: ")
        if word == word[::-1]:
            sleep(3)
            print("\nThis is palindrome")
        else:
            sleep(3)
            print("\nThis isn't palindrome")
    else:
        print("only 1-4!!!\n")
    out = input("\nDo you want to exit? y/n\n ")
    if out == "y" or out == "yes":
        break

print("Thank you and good bye..")
