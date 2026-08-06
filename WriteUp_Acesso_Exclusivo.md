# Decodificando a flag em XOR

O código encontrado no arquivo:

```text
25783566184c44533c5f47583c464742534247533c5945151649
```

é a flag em hexadecimal e criptografada em XOR.

Para decodificar textos em XOR é necessário usar uma chave (key) para encontrar o texto limpo. Porém, caso já se tenha o texto limpo, é possível utilizá-lo como **key** para encontrar a key real da mensagem.

Sabemos que o começo da flag se dá por:

```text
FLAG{
```

Portanto, podemos utilizar essa informação para conseguir a chave necessária para decodificar a flag.

Utilizando o site **[www.dcode.fr/xor-cipher](http://www.dcode.fr/xor-cipher)**, colocamos o texto codificado na aba **"Text to be XORed"** e `FLAG{` na aba **"Use The ASCII Key"**.

Ao fazer isso, encontramos o código:

```text
c4t!c
```

Porém, apenas parte desse código é a chave necessária, já que não sabíamos qual parte do texto codificado era o texto `FLAG{`.

Tentando usar a key "c4t!c" encontramos o código:

```text
FLAG{/p'<$lHg$!g6f0_m14u*
```

Contudo, ao remover o último `c` e usar a key "c4t!" encontramos:

```text
FLAG{x0r_k3y_r3c0v3r_m14u}
```

que é a flag que buscamos.
