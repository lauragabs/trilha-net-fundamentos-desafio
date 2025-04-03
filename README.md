# DIO - Trilha .NET - Fundamentos

[Site DIO](https://www.dio.me)

## Desafio de Projeto: Sistema de Estacionamento

Este projeto foi desenvolvido para o desafio proposto no curso de Fundamentos da trilha .NET da DIO. O objetivo é construir um sistema que gerencie um estacionamento, permitindo cadastrar, remover e listar veículos.

## Contexto

Você foi contratado para criar um sistema para um estacionamento. As principais funcionalidades do sistema são:

- **Cadastrar veículo:** Adicionar a placa do veículo ao estacionamento.
- **Remover veículo:** Remover um veículo e calcular o valor total com base em um preço inicial e preço por hora.
- **Listar veículos:** Exibir todos os veículos atualmente estacionados.

## Especificação

### Classe `Estacionamento`

- **Atributos:**
  - `precoInicial` (decimal): Valor inicial cobrado pela vaga.
  - `precoPorHora` (decimal): Valor cobrado por hora de permanência.
  - `veiculos` (List<string>): Armazena as placas dos veículos estacionados.

- **Métodos:**
  - `AdicionarVeiculo()`: Solicita a placa do veículo e adiciona à lista.
  - `RemoverVeiculo()`: Solicita a placa e, se o veículo estiver estacionado, pede a quantidade de horas para calcular o valor total, removendo o veículo da lista.
  - `ListarVeiculos()`: Exibe os veículos estacionados ou informa que não há veículos se a lista estiver vazia.

### Menu Interativo

O programa apresenta um menu com as seguintes opções:

1. Cadastrar veículo  
2. Remover veículo  
3. Listar veículos  
4. Encerrar o programa  

## Diagrama de Classe

![Diagrama de classe estacionamento](diagrama_classe_estacionamento.png)

## Como Executar

1. **Clone o repositório**:
   ```sh
   git clone https://github.com/lauragabs/trilha-net-fundamentos-desafio.git
   ```
2. **Abra o repositório no Visual Studio Code.**

3. **Restaure as dependências e compile o projeto**:
   ```sh
   dotnet restore
   dotnet build
   ```
4. **Execute o projeto**:
   ```sh
   dotnet run --project DesafioFundamentos/DesafioFundamentos.csproj
   ```

## Considerações

- Certifique-se de que o .NET 6.0 esteja instalado.
- O sistema utiliza entradas e saídas padrão para interagir com o usuário.
- Esse projeto é um desafio de prática para fixar os conceitos básicos em C#.

## Melhorias Futuras

- Validação aprimorada dos dados de entrada.
- Persistência dos dados (armazenamento em banco de dados ou arquivo).
- Inclusão de testes unitários para garantir a robustez do código.

---

Desenvolvido como parte do desafio DIO - Trilha .NET - Fundamentos.