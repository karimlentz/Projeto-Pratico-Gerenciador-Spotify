# 🎵 Gerenciador de Músicas - Spotify 100

![Linguagem C++](https://img.shields.io/badge/Linguagem-C%2B%2B-blue?style=for-the-badge&logo=c%2B%2B&logoColor=white)

[cite_start]Este sistema foi desenvolvido como projeto prático para a disciplina de **Introdução aos Algoritmos** do curso de **Ciência da Computação** da **Universidade Federal de Lavras (UFLA)**[cite: 1, 2, 4]. [cite_start]O objetivo principal é o gerenciamento de uma base de dados das músicas mais tocadas do Spotify, utilizando conceitos avançados de manipulação de arquivos e algoritmos de busca e ordenação[cite: 11, 126].

## 👥 Autores
* [cite_start]**João Pedro Teodoro de Abreu** [cite: 3]
* [cite_start]**Karim Soares Lentz** [cite: 4]
* [cite_start]**Paulo Sérgio Mendes Taciano** [cite: 5]

---

## 📖 Descrição Técnica
[cite_start]O sistema utiliza uma estrutura de dados (`struct Musicas`) para armazenar informações detalhadas sobre cada faixa, incluindo artista, nome da música, ano de lançamento, gênero, streams (em bilhões) e volume médio (dB)[cite: 13, 22].

### Principais Funcionalidades
* [cite_start]**Persistência Híbrida:** Suporte para leitura e escrita em arquivos **CSV** (`spotify100.csv`) e **Binários** (`Spotify100.bin`)[cite: 11, 84, 94].
* [cite_start]**Algoritmos de Busca:** Implementação de **Busca Binária** para localização eficiente por nome da música, artista ou ano[cite: 14, 107].
* [cite_start]**Ordenação Estável:** Uso de **Selection Sort** em vetores auxiliares de índices, permitindo visualizar os dados em diferentes ordens (alfabética ou cronológica) sem alterar a estrutura original do arquivo[cite: 43, 44, 104, 105].
* [cite_start]**Gestão de Registros:** * Inserção de novas músicas com **redimensionamento dinâmico** do vetor (alocação de memória em tempo de execução)[cite: 61, 62, 113].
  * [cite_start]**Remoção Lógica:** As músicas são marcadas como "apagadas" via flag booleana, preservando a integridade dos dados físicos até a exportação final[cite: 31, 39, 40].
* [cite_start]**Exportação Personalizada:** Permite salvar as alterações escolhendo a ordem dos dados (padrão, artista, música ou ano)[cite: 87, 88].

---

## 🛠️ Tecnologias e Bibliotecas
* [cite_start]**Linguagem:** C++ [cite: 11]
* **Bibliotecas Padrão:**
  * [cite_start]`iostream`: Entrada e saída de dados via console[cite: 19].
  * [cite_start]`fstream`: Manipulação e persistência em arquivos[cite: 20].
  * [cite_start]`string` / `cstring`: Tratamento de cadeias de caracteres e conversões[cite: 21].

---

## ⚙️ Como Compilar e Executar

### Pré-requisitos
Certifique-se de ter um compilador C++ (como o `g++`) instalado.

### Compilação
```bash
g++ projetoPratico.cpp -o spotify_manager
