# Os básicos!
## Antes de começar eu peço que você abra o [REGEX](https://regex101.com/) e vá testando um por um pra ver como funciona

## Correspondência Literal:
- Estrutura: 'ABC'
- Textos válidos: ABC

## Ponto (Qualquer Caractere):
- Estrutura 'A.C'
- Textos Válidos: 'ABC', 'AXC', 'ADC' (E assim vai)
- Textos Inválidos: 'ABBC', 'AC', "ABCDE"

## Âncoras (Inicio e final de uma string):
- Estrutura 'ABC$'
- Textos Válidos: 'ABC'
- Textos Inválidos: 'ABCD', '123ABC', "ABCDEF"

## Classes de Caracteres (Intervalos):
- Estrutura '[A-Z]BC'
- Textos Válidos: 'ABC, XBC, ZBC (E assim vai)'
- Textos Inválidos: 'abc', '123BC', "ABCD"

## Quantificadores (Números de ocorrencia):
- Estrutura '{3}[BC]'
- Textos Válidos: 'AAC, AAAC, AAABC'
- Textos Inválidos: 'AC, AAAAAC, ABC'

## Alternancia:
- Estrutura 'A|B'
- Textos Válidos: 'A ou B'
- Textos Inválidos: 'abc', '123BC', "ABCD"

## Grupos de Captura:
- Estrutura '(ABC|DEF)'
- Textos Válidos: 'ABC, DEF'
- Textos Inválidos: 'abc', 'def', "ABCD"

## Meta-caracteres Especiais (Escapados):
- Estrutura '\d{3}'
- Textos Válidos: 'ABC, XBC, ZBC (E assim vai)'
- Textos Inválidos: 'abc', '123BC', "ABCD"
  - (!) Atenção no arquivo [ESCAPADOS](.) você verá alguns dos principais escapados mais comuns

## Quantificador de Zero ou Mais Ocorrências:
- Estrutura: A*B
- Textos Válidos: B, AB, AAB, AAAB,
- Textos Inválidos: C, AC, ABC

## Quantificador de Uma ou Mais Ocorrências:
- Estrutura: A+B
- Textos Válidos: AB, AAB, AAAB, ...
- Textos Inválidos: B, AC, ABC

## Quantificador de Zero ou Uma Ocorrência:
- Estrutura: A?B
- Textos Válidos: AB, B
- Textos Inválidos: AAB, AC, ABC

## Classe de Caracteres Negada:
- Estrutura: [^0-9]
- Textos Válidos: ABC, xyz, !@#
- Textos Inválidos: 123, 456

## Quantificador Preguiçoso:
   - Estrutura: A+?B
   - Textos Válidos: AB, AAB, AAAB, ...
   - Textos Inválidos: B, AC, ABC

## Classe de Caracteres Negada com Espaços:
- Estrutura: `[^ \t\n\r\f\v]+`
- Textos Válidos: `Palavra1`, `Palavra2`
- Textos Inválidos: `Palavra 3`, `Palavra_4`

## Quantificador de Espaços Opcionais:
- Estrutura: `A\s*B`
- Textos Válidos: `A B`, `A   B`
- Textos Inválidos: `AB`, `A123B`

## Quantificador de Intervalo de Repetição Personalizado:
- Estrutura: `A{2,5}B`
- Textos Válidos: `AAB`, `AAAB`, `AAAAB`, `AAAAAB`, `AAAAAAB`
- Textos Inválidos: `AB`, `AAAAAAAB`

## Meta-caractere de Escape para Ponto:
- Estrutura: `www\.example\.com`
- Textos Válidos: `www.example.com`
- Textos Inválidos: `wwwxexampleycom`, `www@example.com`

## Quantificador com Delimitadores Customizados:
- Estrutura: `A;B|C;D`
- Textos Válidos: `A;B`, `C;D`
- Textos Inválidos: `AB`, `CD`

## Alternância com Palavras Inteiras:
- Estrutura: `\b(cat|dog)\b`
- Textos Válidos: `cat`, `dog`
- Textos Inválidos: `cats`, `dogs`

## Classe de Caracteres Negada com Espaços:
- Estrutura: `[^ \t\n\r\f\v]+`
- Textos Válidos: `Palavra1`, `Palavra2`
- Textos Inválidos: `Palavra 3`, `Palavra_4`

## Quantificador de Espaços Opcionais:
- Estrutura: `A\s*B`
- Textos Válidos: `A B`, `A   B`
- Textos Inválidos: `AB`, `A123B`

## Quantificador de Intervalo de Repetição Personalizado:
- Estrutura: `A{2,5}B`
- Textos Válidos: `AAB`, `AAAB`, `AAAAB`, `AAAAAB`, `AAAAAAB`
- Textos Inválidos: `AB`, `AAAAAAAB`

## Meta-caractere de Escape para Ponto:
- Estrutura: `www\.example\.com`
- Textos Válidos: `www.example.com`
- Textos Inválidos: `wwwxexampleycom`, `www@example.com`

(Sim eu repeti algumas coisas, é pra ver se vc tá atento)
