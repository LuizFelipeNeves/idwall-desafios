# Solução: Manipulação de strings

Como resolução deste desafio, procurei fazer um processo de engenharia reversa e entender como a plataforma funciona, e como ocorre o trafego dos dados.
Pois há casos em que é necessario trabalhar com poucos recursos e nem sempre é possivel usar um header browser.
Uma outra abordagem para resolução, seria usar bibliotecas como cheerio, usando selectors, mas neste desafio não utilizei.

## Pré-requisitos
1- Possuir o Nodejs Instalado [Node.js](https://nodejs.org/en/)(10x+) instalado no seu ambiente. Você pode verificar se o possui abrindo o seu terminal e digitando o seguinte comando:

    $ node -version
    
Caso já possua um JDK instalado em seu ambiente, deverá te retornar algo assim: 

    v11.1.0

2- Possuir as dependências, Para instalar e rodar a aplicação. Rode o comando seguinte no terminal dentro da pasta do projeto:

    $ npm install


## Sem Bot, usando o CLI
    $ npm run cli 'cats;brazil'

    $ npm run cli [parametro] => por padrao: 'cats;brazil'


## Bot no Telegram
3- Rode o comando:
    $ npm start

4- Crie um bot no telegram, inicie uma conversa com @BotFather, e logo em seguida use o comando: /newbot,
informe o nome, e logo em seguida você receberá um token.

5- configurando o .env, dentro da pasta do projeto crie um arquivo com o nome .env 
BOT_TOKEN=Seu Token aqui..

6- Envie uma mensagem para o Bot no seguinte formado: /NadaPraFazer cats;brazil

Logo em seguida o bot enviará uma resposta, como no exemplo abaixo:

```
upvotes: 8679 
 subreddit: cats 
 title: My crazy cat every time I change sheet 
 comments: https://old.reddit.com/r/cats/comments/cdwdcg/my_crazy_cat_every_time_i_change_sheet/ 
 thread: https://old.reddit.com/r/cats/comments/cdwdcg/my_crazy_cat_every_time_i_change_sheet/ 

upvotes: 13069 
 subreddit: cats 
 title: My father passed away and left his sweet boy to me. 
 comments: https://old.reddit.com/r/cats/comments/cdscts/my_father_passed_away_and_left_his_sweet_boy_to_me/ 
 thread: https://old.reddit.com/r/cats/comments/cdscts/my_father_passed_away_and_left_his_sweet_boy_to_me/ 

upvotes: 17679 
 subreddit: cats 
 title: RIP Beau, front page cat for a day 
 comments: https://old.reddit.com/r/cats/comments/cdl4df/rip_beau_front_page_cat_for_a_day/ 
 thread: https://old.reddit.com/r/cats/comments/cdl4df/rip_beau_front_page_cat_for_a_day/
```
