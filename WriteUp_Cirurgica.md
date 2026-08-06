## Analisando a Imagem

A imagem fornecida é uma captura de tela do **Taj Mahal** obtida no **Google Street View**.

![Taj Mahal](imagens/tajmahal.png)

## Identificando o Método

A formatação da flag se da por `FLAG{xxxx.xxxx.xxxx}`, oque indica que a resposta ira usar o site **what3words.com**, que divide o mundo em uma grid, cada casa da grid tendo 3 palavras associados a si.

## Resolução

Ao procurar o Taj Mahal, utilizamos a imagem para posicionar o Street View em relação ao monumento, e utilizamos o arbusto e as pessoas como ponto de referencia para encontrar a posição exata em que a print foi tirada.

Ao encontrar a posição exata recebemos o código:

```text
doctor.meaty.doses
```

## Flag

Encontrando então a flag:

```text
FLAG{doctor.meaty.doses}
```
