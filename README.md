
Email=["sureshk98@gmail.com","kumar4@gmail.com","kumar6@gamil.com"]
password=["Suresh98@","Kumar96#","Kumar98&"]
total=dict(zip(Email,password))
#print(total)
compiled_list = list(zip(Email,password))
#print(compiled_list)
username = input("Enter email id ")
for i in Email:
  if username == i:
    print("Access granted!")
    password1 =input("Password")
    for j in password:
      if password1 ==j:
        print("welcome")
        print("login()")
        break
      else:
        print("Exit")
    break

  elif username!=i:
        print("Email is not registred")
        print("New registration")
        import re
        sp="!@#$%^&*()_+=[]{}/?"
        e=input("enter the email id")
        flag=0
        for each in sp:
          if each==e[0]:
            flag=1
          d=re.findall('^\d',e)
          if d!=[]:
            flag=1
          a=re.findall('.+@.\.[a-z]',e)
          if a!=[]:
            flag=1
          if flag==0:
           l=re.findall(".+@.+\.[a-z]",e)
          if l!=[]:
            flag=0
            p=input("enter New Password")
            if not re.findall('[!@#$%^&*()_+=-{}><]',p):
             flag=1
            if not re.findall('[0-9]',p):
              flag=1
            if not re.findall('[a-z]',p):
             flag=1
            if not re.findall('[A-Z]',p):
             flag=1
            if (len(p))<5:
             flag=1
            if (len(p))>16:
             flag=1
            if flag==0:
             print("the password is valid")
             break
        
        break     
      
  else:
           print("the password is invalid ")

Email.append(l)
password.append(p)
print(Email)
print(password)
