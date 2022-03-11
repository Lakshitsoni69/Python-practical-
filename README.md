# Python-practical-
#question 1
def oddsum(n):
    so=0
    print('Odd terms')
    for i in range (1,2*n+1,2):
        print(i,end='\t')
        so+=i
    print('\nSum of odd terms=',so)

def evensum(n):
    se=0
    print('Even terms')
    for i in range (2,2*n+1,2):
        print(i,end='\t')
        se+=i
    print('\nSum of even terms=',se)

n=int(input('How many terms:'))
oddsum(n)

evensum(n)
s=0
n=int(input("enter limit: "))
for i in range(1,n+1):
    s+=i
print("the sum is ",s)

#question2
#(a)
t1=(1,2,5,7,9,2,4,6,8,10)
l=len(t1)
half=l//2
print('First half',t1[:half+1])
print('Second half',t1[half:l+1])
#(b)
print('Another tuple having even numbers from the given tuple')
t2=()
for i in t1:
    if i%2==0:
        t2+=(i,)
print('Tuple containg even numbers:',t2)
#(c)
t1+=(11,13,15)
#(d)
print('concatenated tuple',t1)
print('maximum value',max(t1))
print('minimum value',min(t1))


#question3
def string():
    choice =int(input('''Enter your choice 
1 = length of the string
2 = maximum of three strrings
3 = Replace every successive character with #
4 = number of words in the string
'''))

    if choice == 1:
        n = input("Enter a string : ")
        l=len(n)
        print("The length of the string is =",l)      
    elif choice == 2:
        n1 = input("Enter 1st string : ")
        n2 = input("Enter 2nd string : ")
        n3 = input("Enter 3rd string : ")
        print("The maximum of the three strings is =",max(n1,n2,n3))    
    elif choice == 3:
        n = input("Enter a string : ")
        s = ""
        m = list(n)
        for i in range(len(n)):
            if (i%2 != 0):
                if m[i] == " ":
                    m[i] = " "
                else:
                    m[i] = "#"
        for x in m:
            s=s+x
        print("The sucessive character in the string is replaced with # :",s) 
    elif choice == 4:
            n = input("Enter a string : ")
            c = 0
            for y in n :
                if y == " " :
                    c += 1
            w = c+1
            print("The number of words = ",w) 
    else :
        print("Please Choose from the given option only")

string()
 
