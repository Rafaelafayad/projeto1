# calculadora.py

def soma(a, b):
    return a + b

def subtracao(a, b):
    return a - b

def multiplicacao(a, b):
    return a * b

def divisao(a, b):
    if b == 0:
        return "Erro! Divisão por zero."
    return a / b

if __name__ == "__main__":
    print("Escolha a operação:")
    print("1. Soma")
    print("2. Subtração")
    print("3. Multiplicação")
    print("4. Divisão")
    
    opcao = int(input("Digite o número da operação (1/2/3/4): "))

    num1 = float(input("Digite o primeiro número: "))
    num2 = float(input("Digite o segundo número: "))

    if opcao == 1:
        print(f"{num1} + {num2} = {soma(num1, num2)}")
    elif opcao == 2:
        print(f"{num1} - {num2} = {subtracao(num1, num2)}")
    elif opcao == 3:
        print(f"{num1} * {num2} = {multiplicacao(num1, num2)}")
    elif opcao == 4:
        print(f"{num1} / {num2} = {divisao(num1, num2)}")
    else:
        print("Opção inválida!")
