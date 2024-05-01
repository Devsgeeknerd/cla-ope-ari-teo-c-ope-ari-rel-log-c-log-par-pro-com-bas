<!-- Título -->
# Operadores Aritméticos — Teoria em C

***Conteúdo da Aula:***

Assim como a maioria das linguagens de programação, o **C** possui os seguintes operadores aritméticos:

| Operador | Descrição |
| :------: | :--------:|
| `+` | Operador de adição |
| `-` | Operador de subtração |
| `*` | Operador de multiplicação |
| `/` | Operador de divisão |
| `%` | Operador módulo (resto da divisão) |

Operadores aritméticos só podem ser utilizados com os tipos numéricos, como `int`, `float` e `double`.

Veja o exemplo abaixo:

```C
int main() {
    int a = 2;
    int b = 2;
    // Soma será igual a 4.
    int soma = a + b;
    // Subtração será igual a 0.
    int subtracao = a – b;
    // Multiplicação será igual a 4.
    int multiplicacao = a * b;
    // Divisão será igual a 1.
    int divisao = a / b;
    // Resto será igual a 0 (a divisão de 2 por 2 não deixa resto).
    int resto = a % b;
}
```

Nós podemos somar também constantes numéricas, e não somente variáveis.

Observe o exemplo:

```c
int main() {
    // "a" será equivalente a "5".
    int a = 3 + 2;
    // "b" será equivalente a "8".  
    int b = a + 3;
}
```

Também podemos fazer operações aritméticas entre variáveis de tipos diferentes, porém, o resultado será sempre do tipo de variável **maior**...

Se somarmos um `int` com um `float` o resultado será um `float`; se somarmos um `float` e um `double`, o resultado será um `double`, e assim por diante.

É comum combinar instruções aritméticas em um programa.

Quando isso é feito, cada operador segue as regras de precedência (também chamada de ordem de operadores), que ditam a ordem em que as operações, na mesma instrução, devem ser realizadas.

As regras de precedência básica são as seguintes:

* Expressões entre parênteses são avaliadas primeiro.
  * Se houver mais parênteses, as expressões dentro dos parênteses mais internos são avaliadas primeiro;
* Multiplicação e divisão são avaliadas logo em seguida.
  * Se houver mais de uma no mesmo nível, serão avaliados os operadores da esquerda para a direita;
* Adição e subtração são avaliadas depois.
  * E se houver mais de uma no mesmo nível, serão avaliados os operadores da esquerda para a direita.

Por exemplo, considere as duas expressões abaixo:

```c
int a = 2 + 3 * 4
int b = (2 + 3) * 4
```

Após executadas, a variável `a` terá o valor **14**.

De acordo com as regras de precedência, a multiplicação é realizada antes da adição.

Então, **3** é multiplicado por **4**, resultando **12**; em seguida, é somado **2**, obtendo-se **14**.

Já o valor da segunda expressão será **20**, porque os parênteses forçam a operação de adição a ser realizada primeiro.

Então, **2** é somado a **3**, resultando **5**; em seguida, **5** é multiplicado por **4**, obtendo-se **20**.

<!-- Informações -->
## &#8505; Informações

![Visitors](https://api.visitorbadge.io/api/visitors?path=Devsgeeknerd%2Fcla-ope-ari-teo-c-ope-ari-rel-log-c-log-par-pro-com-bas&label=Visitantes&labelColor=%23700070&labelStyle=none&countColor=%23000fff&style=plastic&color=%23ffffff "Total de Visitantes")
&nbsp;
![Followers](https://img.shields.io/github/followers/Devsgeeknerd?style=p&label=Seguidores&labelColor=800080&color=000fff "Total de Seguidores")
&nbsp;
![Watchers](https://img.shields.io/github/watchers/Devsgeeknerd/cla-ope-ari-teo-c-ope-ari-rel-log-c-log-par-pro-com-bas?style=p&label=Observadores&labelColor=800080&color=000fff "Total de Observadores")
&nbsp;
![Stars](https://img.shields.io/github/stars/Devsgeeknerd/cla-ope-ari-teo-c-ope-ari-rel-log-c-log-par-pro-com-bas?style=p&label=Estrelas&labelColor=800080&color=000fff "Total de Estrelas")
&nbsp;
![Forks](https://img.shields.io/github/forks/Devsgeeknerd/cla-ope-ari-teo-c-ope-ari-rel-log-c-log-par-pro-com-bas?style=p&label=Bifurcações&labelColor=800080&color=000fff "Total de Bifurcações")
&nbsp;
![Repo Size](https://img.shields.io/github/repo-size/Devsgeeknerd/cla-ope-ari-teo-c-ope-ari-rel-log-c-log-par-pro-com-bas?style=p&label=Tamanho&labelColor=800080&color=000fff "Tamanho do Repositório")
&nbsp;
![License](https://img.shields.io/github/license/Devsgeeknerd/cla-ope-ari-teo-c-ope-ari-rel-log-c-log-par-pro-com-bas?style=p&label=Licença&labelColor=800080&color=000fff "Licença do Repositório")
