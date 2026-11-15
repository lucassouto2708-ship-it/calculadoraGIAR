# Apuração da GIAR

Calculadora que apura o valor da GIAR (gratificação da arrecadação) de um mês a partir da arrecadação incrementada e da ARPA, e gera um demonstrativo de cálculo em PDF.

## Como usar

1. Abra `index.html` no navegador (duplo clique).
2. Informe os dados do mês de referência: arrecadação e ARPA.
3. Confira o percentual e o valor calculados.
4. Clique em **Gerar cálculo** para abrir o demonstrativo, com os dados, a memória de cálculo e as hipóteses de exclusão.

## Fórmula usada

Conforme aparece na memória de cálculo do código:

```
%GIAR = 1 + (INCR / ARPA)
Valor = INCR × %GIAR
```

Quando a ARPA é zero, o cálculo não é possível e a página informa isso.

## Correção pela Selic ou por índice

Para o valor de referência, a página monta um link para a calculadora do cidadão do Banco Central, com a correção pela Selic ou por índice, para conferência.

## Arquivos

- `index.html`: a calculadora e o layout do demonstrativo, em um único arquivo.

## Observações

- A página não tem dependências externas além das fontes do navegador e do link para o Banco Central.
- A tema claro/escuro é salvo no navegador (localStorage).
- Confirme a fórmula com a legislação municipal antes de usar o resultado em documento oficial.
