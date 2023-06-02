# FlappyBird
**Recriando o FlappyBird com IA**

Neste projeto o famoso joguinho FlappyBird foi desenvolvido para IA conseguir aprender a vencer em todos os obstáculos. A IA por trás disso 
é chamada de NEAT (Neural Evolution Augmenting Topology) isso é: Ela é uma rede neural que evolui de acordo com o aprendizado. Em resumo o 
jogo foi criado normalmente usando a biblioteca **pygame** e dentro dele foi introduzido a NEAT. A rede neural NEAT funciona atráves de input 
e output. 

> Exemplo: Cada passáro do FlappyBird é uma rede neural 
> Esse passáro precisa receber inputs para devolver um output 
> Ex: Input são as informações que você dá para o passaro para que ele possa tomar uma decisão 
> Output é a decisão que ele tem que tomar. 
> As informações que você vai dar ao passáro como input são informações de como se você estivesse jogando, ou seja, informações da hora de pular, baixar ou levantar 

Os inputs selecionados foram: 

1. Posição Y do pássaro 
2. Distância do passáro para o cano de cima 
3. Distância do passáro para o cano de baixo 

Output: 

Pula? 

1. Sim 
2. Não

A IA - Neat usa como basse de cálculo **input = Output tanH(Output - bias) = resultado da ação, esse resultado da ação pode vir de forma 
aleatória, de 0 à 10 milhões, então é usando a tanH (Função tangente Hiperbólica) para condensar o resultado e se encaixar na regra que 
passamos para o resultado. 

Com a aplicação da NEAT no jogo é criado por volta de 100 passáros para iniciar o jogo, lembrando que cada passáro é uma rede neural.
cada um dos pássaros tomarão uma decisão diferente. Casa pássaro desse tem um valor de baias diferente e um peso diferente. 




