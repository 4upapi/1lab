#Шеснадцатиричные четные числа, не превышающие 2048в10 и содержащие количество цифр равное первой цифре. Вывести числа и их количество. Максимальное число вывести прописью.

buf = ''
ch = ''
max = '0'
col1 = 0
col2 = 0
slov = {0:'ноль',1:'один',2:'два',3:'три',4:'четыре',5:'пять',6:'шесть',7:'семь',8:'восемь',9:'девять',\
     'A':'десять','B':'одинадцать','C':'двенадцать','D':'тринадцать','E':'четырнадцать','F':'пятнадцать'}
with open("text.txt",'r') as f:
    buf = f.readline(1)
    if not buf:
        print("Файл является пустым")
        col2 +=1
    while buf:
        while buf in ['1','2','3','4','5','6','7','8','9','0','A','B','C','D','E','F']:
            ch += buf
            buf = f.readline(1)
        if len(ch) > 0:
            if str(len(ch)) == ch[0] and int(ch,16) % 2 ==0 and int(ch,16) <= 2048:
                col1 += 1
                if int(max,16) < int(ch,16):
                    max = ch
                print(ch, end=' ')
        ch = ''
        buf = f.read(1)
if col1 == 0 and col2 == 0:
        print("Чисел не найдено", end=" ")
print('')
if col1 >0:
    print('Количество чисел:', col1)
    print('Максимальное из чисел:',end=' ')
    for j in range(len(max)):
        for l in slov:
            if str(l) == max[j]:
                print(slov[l], end=' ')
                break
            elif str(l) == max[j]:
                print(slov[l], end=' ')
