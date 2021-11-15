#My first projects using python

print ('TABELA IMC           CLASSIFICAÇÃO \n' 
       'MENOR QUE 18,5:            MAGREZA\n' 
       'ENTRE 18,5 E 24,9           NORMAL\n' 
       'ENTRE 25,0 E 29,9        SOBREPESO\n'
       'ENTRE 30,0 E 39,9        OBESIDADE\n' 
       'MAIOR QUE 40,0     OBESIDADE GRAVE\n')

peso = float(input('Qual é o seu peso em kg ? '))
altura = float(input('Qual é a sua altura em cm ? '))

imc = (round(peso / (altura/100)**2, 2))

if imc < 18.5:
    print (f'Seu IMC é de: {imc}','\n Classificação MAGREZA !!!')

elif imc >= 18.5 and imc < 24.9:
    print (f'Seu IMC é de: {imc}', '\n Classificação NORMAL !!!')

elif imc >= 25.0 and imc < 29.9:
    print (f'Seu IMC é de: {imc}', '\n Classificação SOBREPESO !!!')

elif imc >= 30.0 and imc < 39.9:
    print (f'Seu IMC é de: {imc}', '\n Classificação OBESIDADE !!!')

elif imc > 40.0:
    print (f'Seu IMC é de: {imc}', '\n Classificação OBESIDADE GRAVE !!!')


input()
