# 🎵 Projeto prático - Gerenciador Spotify

![Linguagem C++](https://img.shields.io/badge/Linguagem-C%2B%2B-blue?style=for-the-badge&logo=c%2B%2B&logoColor=white)

Este sistema foi desenvolvido como projeto prático para a disciplina de **Introdução aos Algoritmos** do curso de **Ciência da Computação** da **Universidade Federal de Lavras (UFLA)**. O objetivo principal é o gerenciamento de uma base de dados das músicas mais tocadas do Spotify, utilizando conceitos avançados de manipulação de arquivos e algoritmos de busca e ordenação.

## 👥 Autores
* **João Pedro Teodoro de Abreu**
* **Karim Soares Lentz**
* **Paulo Sérgio Mendes Taciano**

---

## 📖 Descrição Técnica
O sistema utiliza uma estrutura de dados (`struct Musicas`) para armazenar informações detalhadas sobre cada faixa, incluindo artista, nome da música, ano de lançamento, gênero, streams (em bilhões) e volume médio (dB).

### Principais Funcionalidades
* **Persistência Híbrida:** Suporte para leitura e escrita em arquivos **CSV** (`spotify100.csv`) e **Binários** (`Spotify100.bin`).
* **Algoritmos de Busca:** Implementação de **Busca Binária** para localização eficiente por nome da música, artista ou ano.
* **Ordenação Estável:** Uso de **Selection Sort** em vetores auxiliares de índices, permitindo visualizar os dados em diferentes ordens (alfabética ou cronológica) sem alterar a estrutura original do arquivo.
* **Gestão de Registros:** * Inserção de novas músicas com **redimensionamento dinâmico** do vetor (alocação de memória em tempo de execução.
* **Remoção Lógica:** As músicas são marcadas como "apagadas" via flag booleana, preservando a integridade dos dados físicos até a exportação.
* **Exportação Personalizada:** Permite salvar as alterações escolhendo a ordem dos dados (padrão, artista, música ou ano).

---

## 🚀 Tecnologias Utilizadas

- **C++** — Desenvolvimento do programa principal.
- **CSV / Binário** — Manipulação de dados de entrada.

---

## ⚙️ Como Compilar e Executar

```bash
# Compilar o programa (exemplo com g++)
g++ projetoPratico.cpp -o projetoPratico

# Executar, passando os arquivos de dados (se necessário)
./projetoPratico spotify100.csv
# ou, caso utilize o binário:
./projetoPratico Spotify100.bin
```
