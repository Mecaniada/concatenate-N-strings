#Write a Python program
# to concatenate N strings.

import time
li = list()
while True:
    data = input('Enter text:')
    if data == 'restart':
        li = list()
        print('The list has been removed!')
    elif len(data) > 0:
        data = data.strip()
        li.append(data)
        print("The list I've created based on the inserted data:\n\t",li)
    else:
        break
print('Proccesing the received data...\n\tWait a second...')
time.sleep(2)

# look for spaces in word
for word in li:
    x = " "
    if x in word:
        ind = li.index(word)
        print('There were blank spaces inserted at index ' + str(ind) + ".")
        #print(word) # see if the phrase with blank space/s is selected correctly
        word_space0 = word.strip().split()
        print(word_space0)
        li.remove(word)
        for word_sp in word_space0:
            li.append(word_sp)
        print('The final list:\n\t', li)


def conc():
    conc1 = '-'.join(str(word) for word in li)
    return conc1


Master = input('Is there anything else you want me to do?\n\tEnter the process: ')
if Master == 'conc':
    print(conc())
