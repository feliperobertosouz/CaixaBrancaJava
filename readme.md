# Testes de Caixa branca

### Desenvolvedor:
 Felipe Roberto de Souza Silva
 
## Erros encontrados
1-Abertura da conexão do banco de dados não estava sendo fechada corretamente, causando um erro de conexão com o banco de dados.

Local
 - Deveria ser fechado no final do metodo verificarUsuario, mas não existe o fechamento da conexão com o banco de dados

2- Não tratamento correto dos catchs e exceptions

Local
 - Deveria ser tratado os catchs e exceptions, mas não existe o tratamento correto, não existindo nem um "print" da Exception

3- Exposição de informações sensíveis no código fonte (senha e login)

Local
 - Deveria ser criado um arquivo de configuração para armazenar as informações sensíveis, mas não existe o arquivo de configuração, em vez disso as informações foram inseridas dentro de uma string

4- Falta de comentários no código

Local
 - O codigo não possui nenhum comentário, dificultando a manutenção do código

5- Vulnerabilidade pois pode acontecer SQL Injection no código

Local
 - O codigo não possui nenhum tratamento para SQL Injection, podendo causar vulnerabilidade no sistema

6- Quebras do conceito SOLID (Single Responsibility Principle)

Local
 - A classe User possui um metodo que faz conexão com o banco de dados sendo que essa não é uma responsabilidade que essa classe deveria ter

# Miro

[Link para o quadro do Miro](https://miro.com/app/board/uXjVNfZZdbU=/?share_link_id=265233265789)


# Etapa 3
Se você esta vendo isso é porque está na Branch Etapa3

Nessa branch foi feito a documentação do código localizado em [src/login/User](./src/login/User.java) usando as docStrings do javadoc.]

Você pode observar a documentação sendo feita com /** <documentação **/ no código. Isso permitiu ser gerado automaticamente um JavaDoc utilizando
a IDEA InteliJ. 

Para gerar o JavaDoc basta ir em Tools -> Generate JavaDoc e selecionar a pasta src como pasta de origem e a pasta doc como pasta de destino.

Você pode ver o javaDoc ja gerado em [javaDoc/index.html](./javaDoc/index.html)
