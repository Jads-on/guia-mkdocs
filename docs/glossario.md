# Glossário de tecnologias base

## YAML ("YAML Ain't Markup Language")
&emsp; O YAML é uma linguagem de serialização de dados legível por humanos, baseada em indentação, usada principalmente para criar arquivos de configuração, como no MkDocs com o `mkdocs.yml`.

&emsp; Sintaxe básica:

- Utiliza pares Chave: Valor
- Usa dois-pontos (`:`) seguidos obrigatoriamente de um espaço em branco
- Listas são definidas com hífen (`-`)

### YAML vs JSON
&emsp; O YAML é um superconjunto do JSON (qualquer JSON válido é um YAML válido) e evita o uso excessivo de chaves (`{}`), colchetes (`[]`) e vírgulas.

&emsp; Exemplo em YAML:

```yaml
nome: Robocar
versao: 1.0
componentes:
  - motor_dc
  - esp32
  - baterias:
      - 12v
      - 3.3v
```

&emsp; Exemplo equivalente em JSON:

```json
{
  "nome": "Robocar",
  "versao": 1.0,
  "componentes": [
    "motor_dc",
    "esp32",
    {
      "baterias": [
        "12v",
        "3.3v"
      ]
    }
  ]
}
```

## Markdown (.md)
&emsp; Linguagem de marcação leve criada para formatar texto puro de forma intuitiva, sendo facilmente convertida para HTML.

&emsp; Sintaxe básica (exemplo):

```markdown
# Título Principal (H1)
## Subtítulo (H2)

Este é um texto em **negrito** e este em *italico*.

Lista de itens:
- Item 1
- Item 2

[Link para o Google](https://www.google.com)
```

