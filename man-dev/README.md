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
