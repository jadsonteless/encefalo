# Cores & Background

## Tipos:

* background-color (Para caixas)
* border-color (Para caixa)
* color (Para Textos)
* outros...

## Valores:

* Palavras-chaves (blue, transparent)
* Hexadecimal (#990011 | red-green-brue)
* Função; rgb, rgba, hsl, hsla

```css
element {
    /* Exemplo keyword value (palavra-chave) */
    color: currentcolor; /* -> Pega a cor do contesto */

     /* <named-color> values (Colocar a COR digitando o nome) */
    color: blue;
    color: red;
    color: green;
    color: orange;

    /* <hex-color> values (RED-GREEN-BLUE) 0-f (0 a 9 - A a F) */
    color: #000099; /* 00-RED 00-GREEN 99-BLUE (ficou AZUL) */
    color: #00009988; /* 000099|88-alfa (ficou AZUL transparente) */
    color: #0098; /* é o mesmo de 000099|88-alfa (ficou AZUL transparente) OBS!: Quanto mais caracteres mais controle sobre a cor */
        
    /* <rgb()> values (rgb(red-green-blue-alfa) de 0 - 255) */
    color: rgb(255, 0, 0); /* Vermelho intenso */
    color: rgb(255, 0, 0, 0.6); /* Vermelho intenso e um pouco transparente (value alfa add) */
    color: rgb(255, 0, 0, 0.6); /* (alfa em porcentagen) Vermelho intenso e um pouco transparente */
    
    /* <hsl()> values (rgb(hue-saturação-luz-alfa) de 0 - 255) */
    color: rgb(30, 100%, 50%, 20%); /* 30 graus - 100% de saturation - 50% iluminação - 20% de transparencia */

    /* Blobal values */
    color: inherit; /* -> Herda a cor do elemento interior */
    color: initial; /* -> Pega sua cor inicial (root?) */
    color: unset; /* -> Pega sua cor inicial (root?) */
}
```
### Exemplos:
[Exemplo 01](https://encefalo.vercel.app/2-CSS/5-Cores/01-exemplo.html)