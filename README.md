#Projeto de Monitoramento de Temperatura e Umidade

Este é um projeto simples de monitoramento de temperatura e umidade utilizando um sensor DHT11 e um Arduino. O objetivo é monitorar a temperatura e umidade ambiente e emitir alertas caso alguma das medidas ultrapasse limites pré-definidos.

#Pré-requisitos:
Arduino Uno ou similar
Sensor DHT11
LED verde, amarelo e vermelho
Buzzer
Fios jumpers

#Instalação:
Conecte o pino positivo do LED verde ao pino 3 do Arduino, o pino positivo do LED amarelo ao pino 4 do Arduino, o pino positivo do LED vermelho ao pino 5 do Arduino e o pino positivo do buzzer ao pino 6 do Arduino. Conecte o pino negativo de todos os componentes ao GND do Arduino.
Conecte o pino sinal do sensor DHT11 ao pino 2 do Arduino.
Faça o upload do código disponível neste repositório para o seu Arduino.
Utilização

Ao ligar o Arduino, o sensor DHT11 irá medir a temperatura e umidade ambiente cinco vezes e calcular a média. Em seguida, o programa irá comparar as médias com limites pré-definidos e acionar os LEDs e buzzer de acordo com a condição de temperatura e umidade (verde se a condição estiver dentro do limite, amarelo se estiver abaixo do limite ideal, vermelho se estiver acima do limite ideal e o buzzer irá tocar). Se ambos estiverem dentro do limite, apenas o LED verde irá acender. O monitoramento será contínuo enquanto o Arduino estiver ligado.

Notas adicionais
O tempo de leitura do sensor pode ser ajustado alterando o valor do delay no loop principal.
Os limites ideais de temperatura e umidade podem ser ajustados alterando os valores nas condições if/else if no loop principal.
