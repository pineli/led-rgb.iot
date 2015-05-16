Controle de led RGB com Node.JS + socket.io + Johnny-five + Arduino
========================================================

Depois de ver o Meetup do Nodebr de São Paulo, mais especificamente a palestra do Paulo Pires e do Alan, resolvi tirar a poeira do meu Arduino e testar o Jhonny-Five e já aproveitando para baixar o socket.io 1.0 e ver tudo rodando.

## Instalando

    git clone git@github.com:Pineli/Controle-led-rgb.git
    cd Controle-led-rgb
    npm install
    
Teste

    #!javascript
    if (teste = 1) {
      console.log('teste');
    }


Módulos utilizados

* johnny-five
* express
* socket.io

A documentação do Johnny-Five pode ser encontrada [aqui](https://github.com/rwaldron/johnny-five/wiki)


Agora conect seu Arduino no cabo USB, faça o upload do **Example > Firmdata > StandandFirmData**

## Executando

```
node app.js
```
No navegador abra a url:
## Instalando

```
localhost:3000
```
Selecione a cor preferida e a mesma será enviada via Websocket ao NodeJS/Johnny-five e que fará com que o led RGB reproduza a mesma cor, ou cor aproximada, a selecionada.


# Circuito utilizado

![Arduino](https://github.com/Pineli/johnny-five/raw/master/docs/breadboard/led-rgb.png)
[imagem retirada da documentação oficial](https://github.com/rwaldron/johnny-five/blob/master/docs/led-rgb.md) 

# Demonstração

[![ScreenShot](https://i1.ytimg.com/vi/9Fcb31sa3uo/default.jpg)](https://www.youtube.com/watch?v=9Fcb31sa3uo&feature=youtu.be)

## License
Licensed under the MIT license.
