# Welcome to MkDocs

For full documentation visit [mkdocs.org](https://www.mkdocs.org).

## Commands

* `mkdocs new [dir-name]` - Create a new project.
* `mkdocs serve` - Start the live-reloading docs server.
* `mkdocs build` - Build the documentation site.
* `mkdocs -h` - Print help message and exit.

## Project layout

    mkdocs.yml    # The configuration file.
    docs/
        index.md  # The documentation homepage.
        ...       # Other markdown pages, images and other files.


## Exemplos

Aqui você encontrara todas as configurações disponíveis para a utilização na documentação do seu projeto.

### Admonition

Admonition disponiveis:

* Success

Syntax:

    !!! tip "Success"
        Conteudo do Admonition

Result:

!!! tip "Success"
    Conteudo do Admonition

* Info

Syntax:

    !!! note "Info"
        Conteudo do Admonition

Result:

!!! note "Info"
    Conteudo do Admonition

* Warning

Syntax:

    !!! warning "Warning"
        Conteudo do Admonition

Result:

!!! warning "Warning"
    Conteudo do Admonition

* Danger

Syntax:

    !!! danger "Danger"
        Conteudo do Admonition

Result:

!!! danger "Danger"
    Conteudo do Admonition


Utilização com collapse (1)
{ .annotate }

1. O + é utilizado para iniciar com o collapse expandido.

Syntax:

    ???+ note
        Conteuno do Admonition

Result:

???+ note
    Conteuno do Admonition

### Table

Syntax:

    | Left      |   Center      |  Right |
    |:----------|:-------------:|------: |
    | col 1 is  |  left-aligned | $000   |
    | col 2 is  |    centered   | $00    |
    | col 3     | right-aligned | $000   |

Result:

| Left      |   Center      |  Right |
|:----------|:-------------:|------: |
| col 1 is  |  left-aligned | $000   |
| col 2 is  |    centered   | $00    |
| col 3     | right-aligned | $000   |

### Code blocks

Syntax:

    ``` php
        $teste = "teste"
    ```

Result:

``` php linenums="1"
    $teste = "teste"
```

### Diagramas

Syntax: 

    ``` mermaid
    graph LR
        A[Start] --> B{Error?};
        B -->|Yes| C[Hmm...];
        C --> D[Debug];
        D --> B;
        B ---->|No| E[Yay!];
    ```

Result:

``` mermaid
graph LR
    A[Start] --> B{Error?};
    B -->|Yes| C[Hmm...];
    C --> D[Debug];
    D --> B;
    B ---->|No| E[Yay!];
```

Para acessar mais exemplos de diagramas [Clique aqui](https://squidfunk.github.io/mkdocs-material/reference/diagrams/){:target="_blank"}


### Grids

Syntax: 

    <div class="grid cards" markdown>

    - :fontawesome-brands-html5: __HTML__ for content and structure
    - :fontawesome-brands-js: __JavaScript__ for interactivity
    - :fontawesome-brands-css3: __CSS__ for text running out of boxes
    - :fontawesome-brands-internet-explorer: __Internet Explorer__ ... huh?

    </div>

Result:

<div class="grid cards" markdown>

- :fontawesome-brands-html5: __HTML__ for content and structure
- :fontawesome-brands-js: __JavaScript__ for interactivity
- :fontawesome-brands-css3: __CSS__ for text running out of boxes
- :fontawesome-brands-internet-explorer: __Internet Explorer__ ... huh?

</div>


Para acessar mais exemplos de grids [Clique aqui](https://squidfunk.github.io/mkdocs-material/reference/grids/){:target="_blank"}


### Content tabs

Syntax:

    === "C"

        ``` c
        #include <stdio.h>

        int main(void) {
        printf("Hello world!\n");
        return 0;
        }
        ```

    === "C++"

        ``` c++
        #include <iostream>

        int main(void) {
        std::cout << "Hello world!" << std::endl;
        return 0;
        }
        ```

    === "PHP"
        ``` php
        <?php

        declare(strict_types=1);

        echo "Hello World!";
        ```


Result:

=== "C"

    ``` c
    #include <stdio.h>

    int main(void) {
      printf("Hello world!\n");
      return 0;
    }
    ```

=== "C++"

    ``` c++
    #include <iostream>

    int main(void) {
      std::cout << "Hello world!" << std::endl;
      return 0;
    }
    ```

=== "PHP"
    ``` php
    <?php

    declare(strict_types=1);

    echo "Hello World!";
    ```