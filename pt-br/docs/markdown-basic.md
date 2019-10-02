Title: Usando Markdown

# Usando Markdown

A documentação de nossos produtos é produzida utilizando o padrão de liguagem Markdown. O Markdown é uma linguagem de marcação leve que você pode usar para adicionar elementos de formatação a documentos de texto em texto simples. Criado por John Gruber em 2004, o Markdown é agora uma das linguagens de marcação mais populares do mundo.

Veja abaixo algumas opções de sintax que podem ser utilizadas na criação de documentos.

## Sintaxe Básica

Esses são os elementos descritos no documento de design original de John Gruber. Todos os aplicativos do Markdown suportam esses elementos.

| Elemento | Sintaxe Markdown |
|---------|-----------------|
| Título | `# H1` <br/> `## H2` <br/> `### H3` |
| Negrito | `**texto em negrito**`|
|Itálico	| `*texto em itálico*` |
|Bloco de citação	| `> bloco de citação` |
|Lista não ordenada |	`1. Primeiro elemento` <br/> `2. Segundo elemento` <br/> `3. Terceiro elemento` |
|Unordered List	| `- Primeiro elemento` <br/> `- Segundo elemento` <br/> `- Terceiro elemento` |
| Código | `código` |
| Regra horizontal | ``---`` |
| Link | `[título](https://www.exemplo.com)`|
| Imagem | `![alt text](image.jpg)` |


### Cabeçalhos

Estruture seus comentários usando cabeçalhos. Os cabeçalhos segmentam comentários mais longos, facilitando a leitura.

Comece uma linha com um caractere hash # para definir um cabeçalho. Organize seus comentários com subtítulos, iniciando uma linha com caracteres hash adicionais, por exemplo, ####. Até seis níveis de títulos são suportados.

Exemplo:

```html
# Esse é um título H1
## Esse é um título H2
### Esse é um título H3
```

### Negrito/Itálico

Exemplo:

```html
*itálico*
**negrito**
***negrito-itálico***^
```

Resultado:

*itálico*
**negrito**
***negrito-itálico***^

### Citação

### Lista ordenada

1. Arrumar a cozinha
2. Preparar ingredientes
3. Cozinhar coisas deliciosas

### Lista não ordenada

Exemplo:

```html
* Leite
* Pão
    * Grãos integrais
* Manteiga
```

Resultado:

* Leite
* Pão
    * Grãos integrais
* Manteiga

### Código

### Linha Horizontal

### Link

### Imagem


## Sintaxe estendida

Esses elementos estendem a sintaxe básica adicionando recursos adicionais. Nem todos os aplicativos Markdown suportam esses elementos.

