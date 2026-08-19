# pc-lopal
Repositório para armazenar os códigos da aula

# Desafio 1

**Os números da versão 1.0.0 representam respectivamente **

* 1- major (maior)

* 0- minor(menor)

* 0- maintenance (manutenção)

 major- a função do programa mudou significativamente ou uma alteração grande no código

minor- novos recursos adicionados, mas que não alteram nada significativamente

maintenance- apenas correção de bugs

# Desafio 2

## Diferença entre dependencies e devDependencies

* **dependencies**- são programas necessários para um aplicativo funcionar 

* **devDepenedencies**- são programas necessários para o desenvolvimento da aplicação, mas não são necessários para a aplicação funcionar em si 

## Como decidir entre as duas 

* **dependencies**- caso seja uma função que seja necessária para o client 

* **devDepenedencies** caso seja uma função que apenas o desenvolvedor necessite

# Desafio 3

## Significado de ~ e de ^

* **~** - *Aproximadamente equivalente à versão.*
Permite alterações no número na versão desde que não ocorra mudança na versão minor ou major 
    * **Exemplo:** ~1.3.0 permite todas as versões de 1.3.0 até 1.3.99, mas não permite 1.4.0

* **^** - *Compatível com a versão.* permite alteração em todos os números da versão menos no número mais a esquerda
    * **Exemplo:** ^1.4.0 permite todas as versões de 1.4.0 até 1.99.99, mas não permitirá 2.0.0; e ^0.2.0 permite todas as versões de 0.2.0 até 0.2.99

* Quando não se tem o ~ ou o ^ é porquê essa é a versão exata e não pode ser nenhuma outra 
    * **Exemplo:** 1.2.3 vai ser 1.2.3, e **NÃO** pôde ser 1.2.4 ou 1.8.6   

# Desafio 4


## Diferença entre CommonJs e Es Modules
* **CommonJs**

    * Uso de exporte e importe entre arquivos
    * Carrega módulos de forma síncrona, os módulos são carregados antes da execução do próximo código
  * Suportado pelo Node.js mas não pelo navegador 


* **Es Modules**

    * uso de importe e exporte para gerenciar dependências
    * Módulos são carregados de forma assíncrona onde o carregamento é separado, melhorando performance
    * Suportado em Node.js e em navegadores

## Origem

* **CommonJs**

    * Feito com o objetivo de padronizar o server-side, feito pela comunidade

* **Es Modules**

    * padronização oficial do server-side (criado depois do CommonJs)

## Importe e exporte

* **CommonJs**

    * const test = require('test')

      * **Exemplo de exportação** console.log(test.test12('Hello world'))

* **Es Modules**

    * import test from 'test'
      * **Exemplo de exportação** console.log(test.test42('GoodBye world'))