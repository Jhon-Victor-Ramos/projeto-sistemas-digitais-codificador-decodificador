# Projeto Final - Sistemas Digitais (UNICAP)

Este repositório contém o projeto final da disciplina de Sistemas Digitais do curso de Ciência da Computação da Universidade Católica de Pernambuco (UNICAP), ministrada pelo Prof. Wilmer Yecid Córdoba.

## Descrição do Projeto

O objetivo deste projeto foi construir um sistema digital combinacional composto por duas partes principais:

1.  **Codificador:** Converte um número decimal de entrada (0 a 15, representado por 4 bits) para código Gray. A representação binária direta da entrada decimal foi usada como passo intermediário para esta conversão.
2.  **Decodificador:** Utiliza a saída do código Gray gerado pelo codificador para acionar um display de 7 segmentos, exibindo uma sequência específica de 16 letras definida pela equipe.

## Funcionalidades

*   **Entrada:** Um valor decimal de 0 a 15, tipicamente fornecido através de um conjunto de botões no circuito principal (cada botão correspondendo a um valor decimal).
*   **Representação Binária Intermediária:** 4 bits (`BCD3` a `BCD0`) mostrando a representação binária direta da entrada decimal (0-15), utilizada como base para a conversão Gray.
*   **Saída Gray:** 4 bits (`G3` a `G0`) mostrando o código Gray correspondente para a entrada.
*   **Saída 7 Segmentos:** Ativa os segmentos (a-g) de um display para formar letras específicas.
*   **Sequência Exibida:** Conforme a entrada decimal varia de 0 a 15, o display de 7 segmentos exibe as letras da frase: **"UNIVERSIDADE CATÓLICA DE PERNAMBUCO"**. Os padrões visuais das letras foram definidos pelo grupo.
![Representação customizada das letras no display 7-segmentos](Representação%20visual%20escolhida%20pela%20equipe%20para%20display%207-segmentos.png)

## Autores

*   [Camila Danielle Ramos Torquato](https://github.com/camilatorquato)
*   [Jhon Victor Ramos Martins](https://github.com/Jhon-Victor-Ramos)
*   [Rielly Luiza Duarte da Silva](https://github.com/rluizaduarte)

## Ferramentas Utilizadas

*   **Logisim (ou Logisim Evolution):** Para projeto, simulação e validação do circuito digital.
*   **Microsoft Excel:** Para criação e documentação da Tabela Verdade e dos Mapas de Karnaugh.
*   **Google Docs:** Para elaboração do [relatório](https://docs.google.com/document/d/1UVIBaWjSoAdevRTAlSgnUcrOSoP84tw-gWTTC1Gpt-w/edit?usp=sharing).

## Arquivos do Projeto

*   `Projeto - Sistemas Digitais_Final.circ`: Arquivo do circuito principal pronto para simulação no Logisim.
*   `Projeto - Tabelas e Mapas.xlsx`: Planilha contendo a Tabela Verdade completa e os Mapas de Karnaugh utilizados para a simplificação das expressões lógicas.
*   `Relatorio_Final_Sistemas_Digitais.pdf`: Relatório final detalhado do projeto, incluindo objetivos, metodologia, desenvolvimento cronológico, desafios, soluções e artefatos.
*   `README.md`: Este arquivo.

## Como Executar/Visualizar

1.  **Instalação:** Certifique-se de ter o Logisim ou, preferencialmente, o Logisim Evolution instalado em seu computador. (Logisim Evolution é recomendado por ser mais atualizado).
2.  **Download:** Baixe o arquivo `Projeto - Sistemas Digitais_Final.circ` deste repositório.
3.  **Abrir:** Abra o arquivo `.circ` utilizando o Logisim/Logisim Evolution.
4.  **Entradas:** O método principal de entrada no circuito final (`main`) é através de um conjunto de **botões**, onde cada um corresponde a um valor decimal de 0 a 15.
5.  **Interação:** Clique no botão correspondente ao valor decimal desejado (0-15). Pode ser necessário manter o botão pressionado para que a saída se estabilize e seja corretamente propagada pelo circuito.
6.  **Observar Saídas:**
    *   Verifique os LEDs ou probes conectados às saídas BCD e Gray para observar os códigos gerados.
    *   Observe o componente Display de 7 Segmentos para visualizar a letra correspondente da sequência "UNIVERSIDADE CATÓLICA DE PERNAMBUCO" sendo exibida para cada combinação de entrada.

**Nota Importante sobre Execução:**
*   **Logisim Evolution:** É altamente recomendado utilizar o **Logisim Evolution**.
*   **Erro de Biblioteca (TCL):** Se ocorrer um erro referente à biblioteca 'TCL', certifique-se de estar usando uma versão recente do Logisim Evolution. Nenhum arquivo de biblioteca externa `.jar` adicional é requerido para este projeto.

## Desafios e Aprendizados

Um dos principais desafios foi garantir o correto mapeamento lógico entre a saída não-ponderada do código Gray e as entradas do decodificador 7-segmentos, superando a confusão inicial com a ordem sequencial do BCD/decimal. A definição de padrões customizados para representar as letras no display de 7 segmentos foi um exercício importante de design. Adicionalmente, na fase final de integração, surgiu um desafio relacionado a dependências de bibliotecas ('TCL') no Logisim, ressaltando a importância de gerenciar o ambiente de desenvolvimento e garantir a portabilidade dos componentes. O projeto reforçou a importância da validação cuidadosa em cada etapa do processo de design digital.
