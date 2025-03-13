# Pokémon Stats Sorter

Este é um script Python que busca informações de Pokémon na [PokéAPI](https://pokeapi.co/) e os organiza de acordo com um critério escolhido pelo usuário. A ideia é permitir que qualquer pessoa possa comparar Pokémon com base em atributos como ataque, defesa ou velocidade de forma rápida e simples.

## 📌 Funcionalidades
- Permite que o usuário digite os nomes dos Pokémon.
- Busca automaticamente os atributos de **ataque**, **defesa**, **velocidade** e **número da Pokédex** na PokéAPI.
- Organiza os Pokémon com base no critério escolhido pelo usuário.
- Utiliza **kwargs** e **funções lambda** para manipular a ordenação de maneira dinâmica.

## 🔧 Requisitos
- Python 3.6 ou superior
- Biblioteca `requests` (caso não tenha, instale com o comando abaixo)
  ```sh
  pip install requests
  ```

## 🚀 Como usar
1. Clone este repositório ou copie o código.
2. Execute o script Python:
   ```sh
   python pokemon_sorter.py
   ```
3. Digite os nomes dos Pokémon separados por vírgula:
   ```sh
   Digite os nomes dos Pokémon separados por vírgula: pikachu, charizard, bulbasaur
   ```
4. Escolha o critério de ordenação:
   ```sh
   Ordenar por ataque, defesa ou velocidade? ataque
   ```
5. Veja os Pokémon ordenados na tela:
   ```sh
   Pokémon ordenados por ataque:
   #006 Charizard - Ataque: 84
   #025 Pikachu - Ataque: 55
   #001 Bulbasaur - Ataque: 49
   ```

## 📊 Exemplo de Saída
```sh
Digite os nomes dos Pokémon separados por vírgula: pikachu, charizard, bulbasaur
Ordenar por ataque, defesa ou velocidade? velocidade

Pokémon ordenados por velocidade:
#006 Charizard - Velocidade: 100
#025 Pikachu - Velocidade: 90
#001 Bulbasaur - Velocidade: 45
```

## 🛠 Tecnologias utilizadas
- **Python**
- **Requests** para fazer requisições HTTP
- **Funções lambda e kwargs** para manipulação dinâmica de dados

## 🔍 Explicação da abordagem
A escolha da **[PokéAPI](https://pokeapi.co/)** foi feita porque ela contém dados detalhados de cada Pokémon, permitindo acessar estatísticas como ataque, defesa e velocidade. A função **lambda** foi utilizada para permitir a escolha dinâmica do critério de ordenação, tornando o código mais flexível e fácil de manter. Em vez de criar múltiplas funções para cada critério, um dicionário com funções lambda permite que a seleção seja feita de maneira eficiente.

## 🤝 Contribuições
Se quiser sugerir melhorias ou relatar problemas, fique à vontade para abrir um **pull request** ou **issue**.

## 📚 Referências
- [PokéAPI](https://pokeapi.co/)
- [Documentação do Requests](https://docs.python-requests.org/en/latest/)
