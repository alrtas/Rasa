# Sara

Assistente criada com o objetivo de cumprir o desafio proposto pela empresa S***** onde é feito a criação de um Chatbot, utilizando [Rasa](https://rasa.com/) que é uma plataforma conversacional com I.A. embarcada. O mesmo desafio também foi realizado utilizando o ([BLiP](https://www.take.net/) + [WIT](https://wit.ai/)), sendo o BLiP o construtor e orquestrador do fluxo conversacional e o WIT o provedor de processamento de lingaguem natural.


São propostas dois fornecedores diferentes para montagem do fluxo, alguns conceitos não foram aplicados porém uma vez que o fluxo fosse elegivel para publicação deverão ser refatoardos, como a criação de BOTs de apoio para reutilização de sub-bots/sub-sistemas, trazendo partes do BOT que poderão ser comuns para outros fluxos automatizados, como a parte de cadastro de cliente, encerramento e pesquisa de satisfação, termos de uso, atendimento humano. Evitando que haja código duplicado, aumentando a escalabilidade, diminuindo tempos de desenvolvimento e melhorando a confiança geral do fluxo.

## Ecossistema RASA

Alguns caminhos
- Simulador de emprestimo pessoal
  - Quantias fixas de 3.000 | 7.000 | 12.000 | 20.000 | 30.000  
  - Tempos fixos de 12 | 24 | 36 | 48
  - Valores do site
- Atendimeno humano
   - Necessário passar por cadastro, informar
      - Nome
      - CPF (validado matematicamente)    
- FAQ
  - Quem oferece credito?
  - Quais as vantagens? 
  - 2 dúvidas sobre emprestimo pessoal
  - 2 dúvidas sobre emprestimo para autonomo 

Algumas regras de negócio:
- Cliente pode solicitar o atendimento humano a qualquer momento
- Cliente pode encerrar o atendimento a qualquer momento
- Caso o cliente informe que o FAQ não resolveu sua dúvida, irá cair no atendimento humano
- Para ser atendido pelo humano o cliente deverá realizar breve cadastro com nome e CPF e aceite dos termos de privacidade
- Caso cliente não aceite os termos de privacidade também cairá no atendimeno humano
- Ao final do atendimento humano cliente participa de pesquisa de satisfação


## Ecossistema BLiP + WIT
 
 * Acesso fluxo do BLiP disponivel [aqui]( https://portal.blip.ai/application/detail/rasa/home) e do WIT [aqui](https://wit.ai/apps/233957128348188/) 
   *  através do login `sararasa.avaliacao@gmail.com` e senha `Avaliacao@r4s4`.
 * Link para teste do Fluxo disponivel [aqui](https://chat.blip.ai/?appKey=cmFzYTo2MTQ5ODAxNi03Y2QwLTQ3MzktOTBjOC02ZTA3OWMyMGYzN2M=)
### Prototipo de baixa fidelidade
![image](https://user-images.githubusercontent.com/32065208/110889960-e5308180-82cd-11eb-804d-0f5c3727b168.png)



