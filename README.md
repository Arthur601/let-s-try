peso = input("digite o peso: ")
altura = input("digite a altura: ")

try:
    peso = float(peso)
    altura = float(altura)

    print(f"o IMC é: {peso / (altura * altura)}")
except ValueError:
    print("Por favor, insira valores numéricos válidos para peso e altura.")
except ZeroDivisionError:
    print("A altura não pode ser zero. Por favor, insira um valor válido para altura.")
