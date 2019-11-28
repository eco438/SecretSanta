import random,time


def fileopen(lst,txt):
    with open(txt) as f:
        i = 0
        for line in f.read().splitlines():
            lst[line] = i          
            i = i+1
        print(i)
    return lst


def pair(lst):
    valuelist = list(lst.keys())
    random.shuffle(valuelist)
    i = 0
    for key in lst:
        if(lst[key] == valuelist[i]):
            random.shuffle(valuelist)
        lst[key] = valuelist[i]
        i = i +1
    
    return lst

def main():
    start = time.time()
    SecretSantaList = {}
    SecretSantaList = fileopen(SecretSantaList,"SecretSanta.txt")
    SecretSantaList = pair(SecretSantaList)
    print(SecretSantaList)
    end = time.time()
    print(end - start)
    return

main()


    
