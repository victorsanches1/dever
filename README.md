# dever 
#1
def soma_loop(n):
    soma = 0
    operacoes = 0  
    for i in range(1, n + 1):
        soma += i
        operacoes += 1
    return soma, operacoes

def soma_formula(n):
    return n * (n + 1) // 2 

n = int(input("Digite um número inteiro positivo n: "))

soma_loop, num_operacoes = soma_loop(n)
soma_formula = soma_formula(n)

print(f"\nSoma com loop: {soma_loop}")
print(f"contas simples (somas) realizadas: {num_operacoes}")
print(f"Soma com fórmula: {soma_formula}")


#2
senha_correta = "senha123"


max_tentativas = 3

for tentativa in range(1, max_tentativas + 1):
    senha = input(f"Tentativa {tentativa} - Digite a senha: ")
    
    if senha == senha_correta:
        print("Bem-vindo!")
        break
    else:
        print("Senha incorreta.")
else:
    print("Acesso bloqueado.")


#3
notas = []


n = int(input("Digite o número de alunos: "))


for i in range(n):
    nota = float(input(f"Digite a nota do aluno {i+1}: "))
    notas.append(nota)


media = sum(notas) / n


maior_nota = max(notas)
menor_nota = min(notas)


acima_da_media = [nota for nota in notas if nota > media]
percentual_acima = (len(acima_da_media) / n) * 100

print(f"\nMédia da turma: {media:.2f}")
print(f"Maior nota: {maior_nota}")
print(f"Menor nota: {menor_nota}")
print(f"Percentual de alunos acima da média: {percentual_acima:.2f}%")

#4
def busca_linear(lista, nome_procurado):
    for i in range(len(lista)):
        if lista[i].lower() == nome_procurado.lower(): 
            return i
    return -1

nomes = ["Ana", "Bruno", "Carlos", "Daniela", "Eduardo"]

nome_busca = input("Digite o nome a ser buscado: ")


posicao = busca_linear(nomes, nome_busca)

if posicao != -1:
    print(f"Nome encontrado na posição {posicao}.")
else:
    print("Nome não encontrado.")

#5 nao sei
