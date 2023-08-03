# GUESS
def jogo_advinhacao():
    numero_secreto = random.randint(1, 100)
    tentativas = 0

    print("Bem-vindo ao jogo de adivinhação!")
    print("Tente adivinhar o número secreto entre 1 e 100.")

    while True:
        tentativa = int(input("Digite o seu palpite: "))
        tentativas += 1

        if tentativa == numero_secreto:
            print(f"Parabéns! Você acertou o número secreto {numero_secreto} em {tentativas} tentativas.")
            break
        elif tentativa < numero_secreto:
            print("Tente novamente. O número secreto é maior.")
        else:
            print("Tente novamente. O número secreto é menor.")

if _name_ == "_main_":
    jogo_advinhacao()
