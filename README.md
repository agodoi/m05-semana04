# Atendimento do Professor

## Terças e quintas. Professor de horário parcial. Nesses 2 dias, podem contar comigo!

# Semama 04 - Ponte Retificadora e Instrumentação

## Impactos no seu Projeto

* Construção de fontes retificadoras
* Domínio em equipamentos de bancada

## Prática (1) - Teste de Condutividade do Diodo

## Nessa aula prática, vamos montar um relatório organizado e registrar os valores medidos e calculados

### 1) Configuração do Multímetro:

* Ajustar o multímetro para o modo "Teste de Diodo" ou medição de tensão DC. Quando você está na escala de Diodo, o resultado na tela é sempre Volts.
* Medição do Diodo:
*    Conectar as pontas de prova do multímetro nos terminais do diodo:
*    Vermelho no ânodo e preto no cátodo (polarização direta).
*    Preto no ânodo e vermelho no cátodo (polarização reversa).

### Responda:

* (a) O que aconteceu com o valor da tensão na polarização direta?
* (b) O que aconteceu com o valor da tensão na polarização reserva?
* (c) O que aconteceu com o sinal sonoro na polarização direta?
* (d) O que aconteceu com o sinal sonoro na polarização reserva?

## Prática (2) - Teste de Retificação do Diodo (Retificador de Meia Onda)


Monte o circuito abaixo usando 1 diodo **(D)** 1N4007, resistor **(R)** de 1k ohms e um protoboard pequeno.

<img src="https://github.com/agodoi/m05-semana03/blob/main/imgs/oscilas-01.png" width="600">

No desenho há 2 telas de osciloscópio, mas na sua bancada, você vai usar 2 canais **CH1** e **CH2** no mesmo osciloscópio.

[Simulação disponível aqui](https://www.tinkercad.com/things/9RGCbPlLCHo-swanky-uusam/editel?returnTo=https%3A%2F%2Fwww.tinkercad.com%2Fdashboard&sharecode=vf-AVNbVSZOR9WH4_qO6Z_5lJVH93FmJYmTr0_vttfM)

### Responda:


(a) Usando o multímetro de bancada, coloque na escala 20V~ (tensão alternada em 20 volts) e confira se você tem 10V~ na saída do gerador de sinais. Ajuste o knob **AMPL** para **MIN** ou **MAX** até encontrar os 10V~.

(b) Usando o multímetro de bancada na mesma escala 20V~, meça a tensão sobre o **R**. Quanto você encontrou?

(c) Usando o multímetro de bancada, mas agora na escala 2V~, meça a tensão sobre o **D**. Quanto você encontrou?

(d) Agora, comprove matematicamente os valores que você mediu.

(e) Diminua o valor de **AMPL** do gerador de sinais para abaixo de 0,7V~ (use o multímetro de bancada para conferir o valor).

(f) Repita as medições de (c) e (d). O que você conclui?

(g) Volte o valor de AMPL para o máximo, e vamos analisar o comportamento de retificação do D. Compare na sua tela do oscilas, o sinal senoidal original e o retificado, tentando colocar os dois sinais um sobre o outro na sua tela, mexendo no botão **POSITION VERTICAL**. Consegue verificar que metade da onda não está presente no **R**?

## Prática (3) - Medindo corrente elétrica

Nessa aula, vamos confirmar na prática, como se mede corrente elétrica de um circuito.


Insira o multímetro em série no seu circuito Diodo e Resistor para medir o Itotal.

<img src="https://github.com/agodoi/m05-semana03/blob/main/imgs/oscilas-02.png" width="600">



### LEMBRE-SE QUE ESSA MEDIÇÃO PODE QUEIMAR O MULTÍMETRO SE NÃO FEITO CORRETAMENTE!!! Mas não tenha medo...


* Meça a corrente total do circuito retificador meia onda.

Responda:

* (a) A corrente que passa pelo **D** é igual a que passa no **R**?
* (b) Vamos conferir se a corrente está dentro dos limites especificados no datasheet do Diodo 1N4007. Acesse esse site [ALL DATASHEET](https://www.alldatasheet.com/) e busque o PDF do 1N4007, faça o download, e busque pelo valor **Average Rectified Output Current**. Esse é o valor máximo de Itotal que o D suporta na polarização direta.
* Um dado importante: o valor da corrente que você está medindo no multímetro não é real. Por que?

* Porque o multímetro só entende sinais senoidais limpos e perfeitos. O sinal que você está medindo é pulsante e não senoidal.


## Prática (4) - Montando um Retificador de Onda Completa

É muito importante você entender o comportamento das correntes e tensões do circuito abaixo para dominar o funcionamento das fontes de qualquer dispositivo eletrônico.

* Monte o circuito abaixo com **MÁXIMO DE CUIDADO!** SE FECHAR CURTO NO SECUNDÁRIO DO TRAFO, VAI FAZER ESTRAGO
* No lugar da fonte, ligue os fios marcados como secundário. O trafo não tem polaridade nos fios. Ambos fios são iguais.
* Os 4 diodos são 1N4007
* O capacitor é eletrolítico de 2.200uF / 25V
* O regulador de tensão é o 7805
* O resistor é de 1k ohms (marrom preto vermelho)

<img src="https://github.com/agodoi/m05-semana04/blob/main/imgs/circuito-retificador-final.png" width="600">

Após a montagem...

### Responda:

(a) Insira o multímetro na escala de corrente A~ entre o secundário e uma das entradas da ponde de diodo para medir a corrente total. Quanto tem de corrente total?
(b) Insira o multímetro na escala de tensão no secundário do trafo, na escala de V~ para medir a tensão total de entrada. Quanto tem de tensão no secundário?
(c) Coloque o CH1 do oscila nos terminais do secundário do trafo e observe a forma de onda. Qual o tipo de onda você está observando?
(d) Coloque o CH2 do oscila nos terminais do R e observe a forma de onda. Qual o tipo de onda você está observando?
(e) Remova o C do circuito e observe a forma de onda. Qual o tipo de onda você está observando?
(f) Volte o C para o circuito. Insira o multímetro na escala de tensão V~ entre os terminais do R. Quanto tem de tensão?
(g) Insira o multímetro na escala de tensão V= após o regulador de tensão. Quanto tem de tensão?
