# NestJS Github CI

Desafio realizado durante a [Maratona Full Cycle 4.0](http://maratona.fullcycle.com.br/)

Inclui operações de CI utilizando Actions do Github.

## Configurações 
1. Settings/Branches
1. Default branch -> master
1. Rules
    1. Require pull requests reviews before merging
        1. Permite que apenas PRs com reviews sejam aceitos; 
    1. Require review from Code Owners
        1. Exige que tenha ao menos 1 review de 1 Code Owner (não aplicado neste projeto) 
    1. Include admins
        1. Aplica as regras também aos admins
    1. Restrict who can push to matching branches
        1. Define quais usuários podem dar push para este branch (não aplicado neste projeto)
        1. Em branco -> ninguém pode subir algo diretamente para o master
    1. Require status checks to pass before merging
        1. Exige que tenha passado nas Actions que serão selecionadas
        

### Code Owners

Os Code Owners definem quais usuários são "proprietários" de um determinado tipo de código. 

É possível por exemplo dizer que o usuário @joazinho é proprietário de todo o código Typescript e então exigir que as PRs que contenham alteração de código TS sejam revisadas (review) por ele.

Para definir os CO deve-se criar um arquivo chamado *CODEOWNERS* na raiz do projeto.
