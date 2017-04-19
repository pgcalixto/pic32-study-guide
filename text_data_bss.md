
## Flash
* Flash é uma memória em que você pode escrever, assim como a RAM; mas, como a ROM, não é apagada quando desligada.
* Flash contém o código e as variáveis inicializadas (diferente de 0), variáveis `const`

## text
* `text` é o que vai para a Flash
* Quando eu adiciono uma nova função ou uma variável inicializada/constante, o `text` aumenta

## data
* Usado para **dado não-inicializado**.
* Quando você declara uma nova variável (não `const`), o `data` aumenta.
* Quando a variável `int32_t myVar = 0x12345678;` é declarada:
  * `myVar` não é constante, então ela vai parar na RAM.
  * Porém, sua inicialização, `0x12345678`, **é** constante, então vai parar a Flash.
  * Essa inicialização é realizada no `startup code`.
