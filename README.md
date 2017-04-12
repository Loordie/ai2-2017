# ai2-2017
list1


=========== RESTART: C:\Users\student.INFORMATYKA\Desktop\list1.py ===========
match_ends
 OK  got: 3 expected: 3
 OK  got: 2 expected: 2
 OK  got: 1 expected: 1
front_x
 OK  got: ['xaa', 'xzz', 'axx', 'bbb', 'ccc'] expected: ['xaa', 'xzz', 'axx', 'bbb', 'ccc']
 OK  got: ['xaa', 'xcc', 'aaa', 'bbb', 'ccc'] expected: ['xaa', 'xcc', 'aaa', 'bbb', 'ccc']
 OK  got: ['xanadu', 'xyz', 'aardvark', 'apple', 'mix'] expected: ['xanadu', 'xyz', 'aardvark', 'apple', 'mix']
sort_last
  X  got: None expected: [(2, 1), (3, 2), (1, 3)]
  X  got: None expected: [(3, 1), (1, 2), (2, 3)]
  X  got: None expected: [(2, 2), (1, 3), (3, 4, 5), (1, 7)]


list2 

========= RESTART: C:\Users\student.INFORMATYKA\Desktop\pc\list2.py =========
remove_adjacent
 OK  got: [1, 2, 3] expected: [1, 2, 3]
 OK  got: [2, 3] expected: [2, 3]
 OK  got: [] expected: []
linear_merge
 OK  got: ['aa', 'bb', 'cc', 'xx', 'zz'] expected: ['aa', 'bb', 'cc', 'xx', 'zz']
 OK  got: ['aa', 'bb', 'cc', 'xx', 'zz'] expected: ['aa', 'bb', 'cc', 'xx', 'zz']
 OK  got: ['aa', 'aa', 'aa', 'bb', 'bb'] expected: ['aa', 'aa', 'aa', 'bb', 'bb']


string1



======== RESTART: C:/Users/student.INFORMATYKA/Desktop/pc/string1.py ========
match_ends
 OK  got: 3 expected: 3
 OK  got: 2 expected: 2
 OK  got: 1 expected: 1
front_x
 OK  got: ['xaa', 'xzz', 'axx', 'bbb', 'ccc'] expected: ['xaa', 'xzz', 'axx', 'bbb', 'ccc']
 OK  got: ['xaa', 'xcc', 'aaa', 'bbb', 'ccc'] expected: ['xaa', 'xcc', 'aaa', 'bbb', 'ccc']
 OK  got: ['xanadu', 'xyz', 'aardvark', 'apple', 'mix'] expected: ['xanadu', 'xyz', 'aardvark', 'apple', 'mix']
sort_last
 OK  got: [(2, 1), (3, 2), (1, 3)] expected: [(2, 1), (3, 2), (1, 3)]
 OK  got: [(3, 1), (1, 2), (2, 3)] expected: [(3, 1), (1, 2), (2, 3)]
 OK  got: [(2, 2), (1, 3), (3, 4, 5), (1, 7)] expected: [(2, 2), (1, 3), (3, 4, 5), (1, 7)]


string 2



======== RESTART: C:/Users/student.INFORMATYKA/Desktop/pc/string2.py ========
verbing
 OK  got: 'hailing' expected: 'hailing'
 OK  got: 'swimingly' expected: 'swimingly'
 OK  got: 'do' expected: 'do'
not_bad
 OK  got: 'This movie is good' expected: 'This movie is good'
 OK  got: 'This dinner is good!' expected: 'This dinner is good!'
 OK  got: 'This tea is not hot' expected: 'This tea is not hot'
 OK  got: "It's bad yet not" expected: "It's bad yet not"
front_back


warmup1

 def helloworld():
    print("Hello, world!")

def board():
    pion = '|'.join(['  ']*3)
    poziom = '\n{}\n'.format('-'*8)
    print(pion,pion,pion,sep=poziom)
    
def tictactoe():
    pion = 'H'.join(['  |  |  ']*3) + '\n'
    poziom ='H'.join(['--+--+--']*3) + '\n'
    blok = pion.join([poziom]*3)
    separator = '+'.join(['='*8]*3) + '\n'
    print(blok,blok,blok,sep=separator)

def multiples():
    for i in range (0,1002):
        if i%5==0:
            print(i,end=' ')
        elif i%3==0:
            print(i,end=' ')
        i=i+1

def collatz(number):
    if number%2==0:
        print(number, "->", end=' '),
        number=number/2        
        collatz(number)
    elif number%2==1:
        if number==1:
            print(number)
        else:
            print(number, "->", end=' '),
            number=3*number+1            
            collatz(number)

def ftoc(temp):
    celsius = (temp - 32) * (5/9)
    print(celsius)
    

ftoc(88)
