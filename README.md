# Projetos
alunos = []

def cadastrar_aluno():
    nome = input("Digite o nome do aluno: ")
    alunos.append(nome)
    print(f"{nome} foi cadastrado com sucesso!\n")

def listar_alunos():
    if len(alunos) == 0:
        print("Nenhum aluno cadastrado.\n")
    else:
        print("\nLista de Alunos:")
        for i, aluno in enumerate(alunos, start=1):
            print(f"{i}. {aluno}")
        print()

def remover_aluno():
    listar_alunos()

    if len(alunos) > 0:
        numero = int(input("Digite o número do aluno para remover: "))

        if 1 <= numero <= len(alunos):
            removido = alunos.pop(numero - 1)
            print(f"{removido} foi removido.\n")
        else:
            print("Número inválido.\n")

while True:
    print("=== SISTEMA DE ALUNOS ===")
    print("1 - Cadastrar aluno")
    print("2 - Listar alunos")
    print("3 - Remover aluno")
    print("4 - Sair")

    opcao = input("Escolha uma opção: ")

    if opcao == "1":
        cadastrar_aluno()

    elif opcao == "2":
        listar_alunos()

    elif opcao == "3":
        remover_aluno()

    elif opcao == "4":
        print("Sistema encerrado.")
        break

    else:
        print("Opção inválida.\n")


# Sistema de Cadastro de Alunos

Projeto desenvolvido em Python para praticar lógica de programação.

## Funcionalidades
- cadastrar alunos
- listar alunos
- remover alunos

## Tecnologias
- Python
- Git
- GitHub
- 


        
