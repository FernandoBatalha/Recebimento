Recebimento
===========

from datetime import datetime
now = datetime.now()

nome = str(input("Digite o Nome: "))
valor = float(input("Digite o Valor: "))
valordodesconto = int(input("Desconto: "))
juro = int(input("Digite o Juro: "))
saida = valor*juro/100
resultado1 = valor + saida


desconto = valor*valordodesconto/100

valordias = float(input("Valor ao Dia: "))
dias = int(input("Quantos dias de Atraso: "))
resultado2 = dias*valordias

total = resultado1 + resultado2 - desconto


print("-"*35)
print("")
print("A RECEBER".center(35))
print("-"*35)
print ("Valor: R$ %.2f"% valor)
print("-"*35)
print("Valor do Desconto: (-) R$ %.2f"%desconto)
print("-"*35)
print ("Juros: (+) R$ %.2f"% saida)
print("-"*35)
print("Multa do Atraso: (+) R$ %.2f"% resultado2)
print("-"*35)
print("")
print (">>> Total a Receber: (=) R$ %.2f"% total)
print("")
print("-"*35)

print (now.day,"/",now.month,"/",now.year,"-",now.hour,":", now.minute,":", now.second)
