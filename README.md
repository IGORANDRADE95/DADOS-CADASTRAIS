# DADOS-CADASTRAIS
Lê os dados cadastrais e faz validações.
nome = str(input("Digite o nome: (Mínimo de 3 caracteres)"))
idade = int(input("Digite a idade: (entre 0 e 150 anos)"))
salario = float(input("Digite o salário: "))
sexo = str(input("Digite sexo: (F ou M)"))
estado = str(input("Digite o estado civil: (s, c, v ou d)"))

while len(nome)<3:
  print("Erro! O nome deve ter mais de 3 caracteres")
  nome = str(input("Digite o nome: (Mínimo de 3 caracteres)"))
  idade = int(input("Digite a idade: (entre 0 e 150 anos)"))
  salario = float(input("Digite o salário: "))
  sexo = str(input("Digite sexo: (F ou M)"))
  estado = str(input("Digite o estado civil: (s, c, v ou d)"))

while idade<0 or idade>150:
  print("Erro! A idade deve estar entre 0 e 150 anos")
  idade = int(input("Digite a idade: (entre 0 e 150 anos)"))
  salario = float(input("Digite o salário: "))
  sexo = str(input("Digite sexo: (F ou M)"))
  estado = str(input("Digite o estado civil: (s, c, v ou d)"))

while salario<0:
  print("Erro! O salário deve ser maior que zero")
  salario = float(input("Digite o salário: "))
  sexo = str(input("Digite sexo: (F ou M)"))
  estado = str(input("Digite o estado civil: (s, c, v ou d)"))
        
while sexo!="f" or sexo!="m":
  print("Erro! O sexo deve ser F ou M")
  sexo = str(input("Digite sexo: (F ou M)"))
  estado = str(input("Digite o estado civil: (s, c, v ou d)"))

while estado!="s" or estado!="c" or estado!="v" or estado!="d":
  print("Erro! O estado civil deve ser s, c, v ou d")
  estado = str(input("Digite o estado civil: (s, c, v ou d)"))
