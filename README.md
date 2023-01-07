# schelling-introverty
Trabalho de Compuração Experimental


Foi adicionado ao modelo de schelling de segregação uma nova variavel, no caso introvertido, com intuito de verificar de os introvertidos ajudariam a criar equilibrio no sistema e reduzir a clusterização do sistema.

Hipotese: Introvertidos podem ajudar a reduzir os clusters do sistema.

Justificativa: Conforme novas variaveis forem adicionadas ao sistema, poderemos averiguar se elas são relevantes ou não para o sistema, como também se são beneficas para o equilibrio dele.


Orientações:
```python3 run.py```
Mudar as variaveis de acordo com o desejado

Homophily: quantas pessoas do mesmo "tipo" o agente precisa ter para ficar feliz

minotiry_pc: % de agentes que vai ser de um determinado tipo no sistema

introverty_limit: % de pessoas do sistema que são introvertidos

similar: vai determinar se a pessoa deve se mover caso ``` smilar < homophily ```

A variavel adicionada ao sistema foi introverty_limit, inicialmente deveria simular o comportamento de uma pessoa introvertida, que tende a ficar longe de grupos de pessoas. Para o algoritmo foi adicionada a seguinte condição: caso alguem esteja perto de um introvertido a similaridade dessa pessoa vai reduzir, caso ele esteja perto de alguem do mesmo tipo que ele a similaridade aumentará, ou seja, caso uma pessoa esteja proxima a um introvertido ficará com -1 de similar, caso uma pessoa esteja proxima a um introvertido que seja do mesmo tipo que ela ficara com 0 de similar. Em ambientes com homofilia muito alto é esperado que os introvertidos não entrem em equilibrio. 

Conforme foi feita a leitura do experimento notei que os introvertidos na verdade estavam tendo um comportamento mais proximo de "radicais", ficando totalmente isolados de tipos diferentes dos deles e ficando no meio dos seus iguais. Notei que o numero de clusteres diminuiram nos experimentos porém que em muitos casos o numero de interações aumentou significativamente. 



