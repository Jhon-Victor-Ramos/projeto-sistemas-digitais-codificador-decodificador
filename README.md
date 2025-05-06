# Projeto Final - Sistemas Digitais (UNICAP)

Este repositório contém o projeto final da disciplina de Sistemas Digitais do curso de Ciência da Computação da Universidade Católica de Pernambuco (UNICAP), ministrada pelo Prof. Wilmer Yecid Córdoba.

## Descrição do Projeto

O objetivo deste projeto foi construir um sistema digital combinacional composto por duas partes principais:

1.  **Codificador:** Converte um número decimal de entrada (0 a 15, representado por 4 bits) para seus equivalentes nos códigos BCD 8421 (para as entradas 0-9) e Gray (para todas as entradas 0-15).
2.  **Decodificador:** Utiliza a saída do código Gray gerado pelo codificador para acionar um display de 7 segmentos, exibindo uma sequência específica de 16 letras definida pela equipe.

## Funcionalidades

*   **Entrada:** 4 bits (A, B, C, D) representando o valor decimal de 0 a 15.
*   **Saída BCD:** 4 bits (`BCD3` a `BCD0`) mostrando o código BCD correspondente (válido para entradas 0-9).
*   **Saída Gray:** 4 bits (`G3` a `G0`) mostrando o código Gray correspondente para a entrada.
*   **Saída 7 Segmentos:** Ativa os segmentos (a-g) de um display para formar letras específicas.
*   **Sequência Exibida:** Conforme a entrada decimal varia de 0 a 15, o display de 7 segmentos exibe as letras da frase: **"UNIVERSIDADE CATÓLICA DE PERNAMBUCO"**. Os padrões visuais das letras foram definidos pela equipe.

## Autores

*   [Camila Danielle Ramos Torquato](https://github.com/camilatorquato)
*   [Jhon Victor Ramos Martins](https://github.com/Jhon-Victor-Ramos)
*   [Rielly Luiza Duarte da Silva](https://github.com/rluizaduarte)

## Ferramentas Utilizadas

*   **Logisim (ou Logisim Evolution):** Para projeto, simulação e validação do circuito digital.
*   **Microsoft Excel:** Para criação e documentação da Tabela Verdade e dos Mapas de Karnaugh.
*   **Google Docs:** Para elaboração do relatório.

## Arquivos do Projeto

*   `Projeto - Sistemas Digitais_Final.circ`: Arquivo do circuito principal pronto para simulação no Logisim.
*   `Projeto - Tabelas e Mapas.xlsx`: Planilha contendo a Tabela Verdade completa e os Mapas de Karnaugh utilizados para a simplificação das expressões lógicas.
*   `Relatorio_Final_Sistemas_Digitais.pdf`: Relatório final detalhado do projeto, incluindo objetivos, metodologia, desenvolvimento cronológico, desafios, soluções e artefatos.
*   `README.md`: Este arquivo.

## Como Executar/Visualizar

1.  **Instalação:** Certifique-se de ter o Logisim ou, preferencialmente, o Logisim Evolution instalado em seu computador. (Logisim Evolution é recomendado por ser mais atualizado).
2.  **Download:** Baixe o arquivo `Projeto - Sistemas Digitais_Final.circ` deste repositório.
3.  **Abrir:** Abra o arquivo `.circ` utilizando o Logisim/Logisim Evolution.
4.  **Entradas:** Localize os 4 pinos de entrada no circuito, geralmente rotulados como A, B, C, D (ou In0 a In3). Estes representam o número decimal de entrada (A sendo o bit mais significativo).
5.  **Interação:** Clique nos pinos de entrada para alternar seus valores (0 ou 1), formando assim as combinações de 0000 (Decimal 0) a 1111 (Decimal 15).
6.  **Observar Saídas:**
    *   Verifique os LEDs ou probes conectados às saídas BCD e Gray para observar os códigos gerados.
    *   Observe o componente Display de 7 Segmentos para visualizar a letra correspondente da sequência "UNIVERSIDADE CATÓLICA DE PERNAMBUCO" sendo exibida para cada combinação de entrada.

## Desafios e Aprendizados

Um dos principais desafios foi garantir o correto mapeamento lógico entre a saída não-ponderada do código Gray e as entradas do decodificador 7-segmentos, superando a confusão inicial com a ordem sequencial do BCD/decimal. Além disso, a definição de padrões customizados para representar as letras no display de 7 segmentos foi um exercício importante de design dentro das limitações da ferramenta. O projeto reforçou a importância da validação cuidadosa em cada etapa do processo de design digital.
