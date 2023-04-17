
# Exercício E2 - Aquecimento com Bison 

- Alterar calc.y para criar regras de produção para a gramática:
``` 
calc -> expr EOL
;

expr -> expr + expr
     |  expr - expr
     |  ( expr )
     |  NUM
;
```
- Alterar calc.y para definir novo(s) token(s), se necessário;
- Alterar calc.y para usar nas regras de produção os nomes de tokens definidos com %token
- Criar um novo arquivo, ```main.c''' e mover a função main() para esse arquivo e alinhar APIs.
- Modificar a função main() para chamar yyparse() e não mais yylex();
- Rodar flex, bison (```bison -d calc.y''') e gerar executável ``calc''.

*Importante*: Aceitar convite enviado via Github Classroom e submeter sua resposta via repositório criado automaticamente para este exercício Github Classroom.  Respostas em repositórios pessoais não serão consideradas.
