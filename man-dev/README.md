# Manual do Desenvolvedor - CRIPTAS DO IFSC

![Criptas do IFSC Logo](https://github.com/PJI29001/treasure-hunt/blob/master/img/logo-criptas.jpeg)

 Olá Desenvolvedor! Nesta página você verá como foi feito o aplicativo Criptas do IFSC e também os pontos cardeais e respostas dos enigmas. Vamos lá!

- [Ferramentas e Requisitos](#ferramentas-e-requisitos)
- [Protótipo](#prototipo)
- [Design](#design)
- [Programação](#programacao)
- [Manuais](#manuais)
- [Agradecimentos](#agradecimentos)

---

## Ferramentas e Requisitos

O aplicativo foi feito na plataforma [App Inventor](http://appinventor.mit.edu/explore/). A programação é toda em blocos, na interface do site App Inventor, feita por meio de um **browser atualizado (Chrome ou Firefox)** em qualquer computador e **não é necessário um computador muito potente** para usá-la. Durante a programação (falaremos mais detalhadamente sobre ela mais abaixo) você precisará de um meio de testar o aplicativo que está sendo criado. Isso pode ser feito usando um **dispositivo móvel operacional com Android versão 2.3 ou superior** ou, opcionalmente, o [Emulador App Inventor](http://appinventor.mit.edu/explore/ai2/setup-emulator.html) ou qualquer outro emulador de android para o seu sistema operacional, onde você possa instalar o .apk nele.

Para a criação do protótipo, pode ser usado o site [draw.io](https://www.draw.io/).

Na confeccção do design (imagens e áudios) foram usados os softwares:

- Adobe photoshop CS6 64bits;
- Dungeon Builder;
- onlinevideoconverter.com;
- Tinypng.

Para recolhimento das coordenadas, usamos o aplciativo Mobile Topographer, disponível na play store para download gratuito.

---

## Protótipo

![Protótipo](https://github.com/PJI29001/treasure-hunt/blob/master/img/prototype.png)

O protótipo acima foi criado com imagens internas do próprio [draw.io](https://www.draw.io/). Nela, é possível ver todas as páginas funcionanis do aplicativo, o *flow* do usuário entre as páginas e a disposição do conteúdo.

---

## Design

### Botões, Páginas e Logo

As imagens de botões para o aplicativo foram criadas com o Adobe Photoshop CS6.

![Botão Avançar](https://github.com/PJI29001/treasure-hunt/blob/master/img/bot-advance.png)

![Botão Confirmar](https://github.com/PJI29001/treasure-hunt/blob/master/img/bot-confirm.png)

![Botão Fase 1](https://github.com/PJI29001/treasure-hunt/blob/master/img/bot-fase1.png)

![Botão Fase 2](https://github.com/PJI29001/treasure-hunt/blob/master/img/bot-fase2.png)

![Botão Fase 3](https://github.com/PJI29001/treasure-hunt/blob/master/img/bot-fase3.png)

![Botão Fase 4](https://github.com/PJI29001/treasure-hunt/blob/master/img/bot-fase4.png)

![Botão Fase 5](https://github.com/PJI29001/treasure-hunt/blob/master/img/bot-fase5.png)

![Botão Fase 6](https://github.com/PJI29001/treasure-hunt/blob/master/img/bot-fase6.png)

![Botão Fase 7](https://github.com/PJI29001/treasure-hunt/blob/master/img/bot-fase7.png)

![Botão Instruções](https://github.com/PJI29001/treasure-hunt/blob/master/img/bot-instructions.png)

![Botão Latitude](https://github.com/PJI29001/treasure-hunt/blob/master/img/bot-latitude.png)

![Botão Play](https://github.com/PJI29001/treasure-hunt/blob/master/img/bot-play.png)

![Botão Retry](https://github.com/PJI29001/treasure-hunt/blob/master/img/bot-retry.png)

### Mapa

O mapa foi criado com o software de criação de mapas para RPG Dungeon Builder. É um software pago, assim como o Photoshop, e pode ser baixado pela Steam. Atualmente ele custa em torno de 30 reais.
Tínhamos a necessidade de representar o terreno do IFSC por um mapa e a criação pelo software foi a mais interessante para nós, suprindo as necessidades e também combinando com o tema medieval do aplicativo.

O mapa de rascunho que usamos para a criação do principal pode ser visto abaixo:

![Mapa de Rascunho](https://github.com/PJI29001/treasure-hunt/blob/master/img/mapa-ifsc.png)

O resultado, após o uso do Dungeon Builder (e já com moldura adicionada), que é mostrado apenas após conclusão de todos os desafios foi:

![Mapa do IFSC](https://github.com/PJI29001/treasure-hunt/blob/master/img/map-moldura.png)

Para a transição entre as fases decidimos usar uma versão com *fog* do mapa pronto:

![Mapa com Fog](https://github.com/PJI29001/treasure-hunt/blob/master/img/map-fog.png)

### Logo

Também criada com o Photoshop, a logo seguiu o tema medieval. As imagens que a compoe foram encontradas no Google.

![Logo Criptas](https://github.com/PJI29001/treasure-hunt/blob/master/img/logo-criptas.jpeg)

Para o ícone mantivemos o escudo da logo e colocamos um a inicial do aplicativo, para dar destaque e ser visível mesmo que pequena.

![icon](https://github.com/PJI29001/treasure-hunt/blob/master/img/icon.png)

---

## Programação

A programação foi feita na plataforma Mit App Inventor, no formato de blocos. Iremos explicar brevemente a composição dos blocos de cada uma das telas do aplicativo.

O aplicativo é composto por 7 fases. Cada uma das fases possui dicas para uma localização específica e um enigma, que só é desbloqueado quando o usuário insere nos espaços Latitude e Longitude as coordenadas corretas.

**OBS**: Os textos mostrados dentro dos blocos não condizem com os textos finais. A programação de blocos foi finalizada antes da criação das dicas.

### Tela 1

A primeira tela é a home do aplicativo. Ela possui os botões `jogar`, `sair do jogo` e `instruções`.

Sua composição é bastante simples, como pode ser vista abaixo:

![Blocos Tela 1](https://github.com/PJI29001/treasure-hunt/blob/master/img/prog/prog-screen1.png)

Esta página tem, como funções, inicializar o banco de dados TinyDB1 e abrir novas screens de acordo com o botão apertado.

### Tela 2

Esta é a tela que abre quando clicamos nas instruções. Ela mostrará uma imagem com o texto de instruções e dará as opções de voltar para a tela anterior e seguir para a fase 1.

![Blocos Tela 2](https://github.com/PJI29001/treasure-hunt/blob/master/img/prog/prog-screen2.png)

### Tela 3

Aqui é onde a mágica acontece. Esta é a página por trás de todas as fases do aplicativo. A cada nova fase, o conteúdo mostrado na tela é resgatado de acordo com o número armazenado no banco de dados. Cada vez que o usuário passa de fase, é adicionado `+1` a nossa global `fase`. De acordo com essa variável `fase`, diferentes imagens e textos aparecerão na tela. Mas vamos por partes.

![Blocos Tela 3 pt1 1](https://github.com/PJI29001/treasure-hunt/blob/master/img/prog/prog-screen3-pt1.png)

Nos blocos da imagem acima, podemos ver todas as variáveis sendo inicializadas na tela e um bloco grande que é responsável por chamar as legendas 1 e 2 e também a imagem da fase armazenada na variável `fase`. podemos ver também um padrão de repetição, pois o processo é o mesmo para cada uma das fases. O que muda entre elas é a legenda e a imagem respectiva.

![Bloco Tela 3 pt2 2](https://github.com/PJI29001/treasure-hunt/blob/master/img/prog/prog-screen3-pt2.png)

Os blocos acima são responsáveis pela parte de coordenadas. Os primeiros 4 blocos laranjas chamam a variável longitude e latitude, dizendo o formato que a resposta deve ser dada e o número de casas.
Após, ele pega as latitudes específicas de acordo com a global `fase`. Se a latitude e longitude forem iguais as especificadas, é aberta uma nova tela de acerto. Caso contrário, o usuário ouvirá o Som 1. O mesmo processo se repete para cada uma da fases.

![Bloco Tela 3 pt 3](https://github.com/PJI29001/treasure-hunt/blob/master/img/prog/prog-screen3-pt3.png)

Os blocos acima são referentes ao botão avanças, contido na tela das fases, e é responsável por mostrar as dicas do local onde serão recolhidos os dados de latitude e longitude. Novamente, a variável de fase será consultada para mostrar as dicas corretas da fase. Cada vez que o usuário apertar o botão avançar, ele verá a próxima dica do local.

### Tela 4

A tela 4 é a mostrada para o usuário após as 7 fases, quando ele poderá responder ao enigma final. É inicializada a global fase e o botão próxima fase envia o usuário para a tela do enigma final.

![Bloco Tela 4](https://github.com/PJI29001/treasure-hunt/blob/master/img/prog/prog-screen4.png)

### Tela 5

A tela 5 é onde serão mostrados para o usuários os enigmas que contém questões de múltipla escolha. Serão 4 botões disponíveis para o usuário, onde caso ele escolha o botão correto, será enviado para a próxima fase. Caso escolha o botão errado, será enviado para a fase anterior. Nota-se que na dase 3, o botão correto é o de número 3, que enviará o usuário para a tela das fases. Qualquer outro botão iria subtrair 1 da variável `fase`, e retornaria para uma tela de erro.

![Bloco Tela 5]

## Manual
