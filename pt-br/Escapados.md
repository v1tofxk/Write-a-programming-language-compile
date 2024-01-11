\d:
   - **Descrição:** Corresponde a qualquer dígito (0-9).
   - **Exemplo:** `\d{3}` corresponde a três dígitos consecutivos.

\D:
   - **Descrição:** Corresponde a qualquer caractere que não seja um dígito.
   - **Exemplo:** `\D+` corresponde a uma ou mais ocorrências de caracteres não dígitos.

\w:
   - **Descrição:** Corresponde a qualquer caractere alfanumérico (equivalente a `[a-zA-Z0-9_]`).
   - **Exemplo:** `\w+` corresponde a uma ou mais ocorrências de caracteres alfanuméricos.

\W:
   - **Descrição:** Corresponde a qualquer caractere que não seja alfanumérico.
   - **Exemplo:** `\W*` corresponde a zero ou mais ocorrências de caracteres não alfanuméricos.

\s:
   - **Descrição:** Corresponde a qualquer caractere de espaço em branco (como espaço, tabulação, nova linha).
   - **Exemplo:** `\s` corresponde a um único caractere de espaço em branco.

\S:
   - **Descrição:** Corresponde a qualquer caractere que não seja de espaço em branco.
   - **Exemplo:** `\S+` corresponde a uma ou mais ocorrências de caracteres não espaços em branco.

\b:
   - **Descrição:** Corresponde a uma posição de fronteira de palavra (início ou fim de uma palavra).
   - **Exemplo:** `\bword\b` corresponde à palavra "word" como uma palavra inteira.

\B:
   - **Descrição:** Corresponde a uma posição que não é uma fronteira de palavra.
   - **Exemplo:** `\Bword\B` corresponde à palavra "word" apenas quando não está isolada como uma palavra inteira.
