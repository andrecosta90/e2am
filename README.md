"Costumo dizer que a sociologia é uma arte marcial, um meio de auto-defesa. Basicamente, você a usa para se defender, sem ter o direito de usá-la para ataques injustos" _Pierre Bourdieu_

##*E2AM* 
_Espada e Escudo Anti Manipulação_

**O que é:** Um projeto [FOSS][foss] em nome de um verdadeiro pensamento livre. 

**Problema:** Mesmo buscando informações na internet muitas vezes sua opinião é decidida por um grupo de jornalistas, políticos ou marketeiros. Não é fácil identificar o verdadeiro impacto da mídia.

**Proposta:** Empregar técnicas de [mineração de texto][mine] e [abstração de sentimento][abst] para cruzar dados vindos de feeds de notícia e redes sociais. Dessa forma será possível identificar em tempo real padrões e discrepâncias entre o que dizem as pessoas e os canais de notícia, podendo então quantificar e qualificar o impacto de determinados assuntos e canais de notícia na opinião pública, bem como tentativas deliberadas para guiar o pensamento de um grupo de pessoas para uma opinião em comum.

Mais detalhamente, será possível discernir grupos tanto de pessoas quanto de canais de notícia por seus interesses. Assim padrões serão facilmente identificáveis, por exemplo, o algoritmo deverá perceber que os interesses da Veja são compatíveis com os interesses do PSDB e também com um grupo de médicos. Esses grupos tenderiam a concordar na maioria dos casos e poderiam talvez influenciar outros grupos, como foi o caso das manifestações de Junho em São Paulo. 

Se eu percebesse o quanto estava sendo manipulado, provavelmente minha participação nos protestos teria sido diferente. Perceber a manipulação é a parte que considero o "escudo" para proteger um pensamento crítico legítimo. 

A parte agressiva do software (a "espada") usaria o mesmo mecanismo de mineração de opinião e sentimento, mas nesse caso seria para rastrear notícias relacionadas a corrupção, os políticos e partidos envolvidos e a opinião dos canais de notícias em relação a isso. Seria então possível visualizar facilmente quais canais de notícia estão tentando derrubar ou eleger determinados políticos e legendas e também classificar os políticos mais vinculados a casos de corrupção. 

**Algumas premissas:** O projeto será desenvolvido em [Python 2.7][pyth], utilizando o paradigma de [computação paralela][para] com [octo.py][octo] em nome da escalabilidade, já que haverá mais dados para analisar do que prevê a vã programação tradicional. Para análise de sentimento será usado o [Classificador Ingênuo de Bayes][baye], [TF-IDF][tfid] e provavelmente [MongoDB][mong] ou mesmo [JSON][json] para armazenar os dados processados de forma estruturada.O software estará sob a licença [GPLv3][gpl3], sendo que os dados utilizados na análise apresentada  **deverão** estar disponíveis para quem quiser fazer o download e testá-los em seu próprio computador. Restringir acesso aos dados seria extremamente prejudicial, pois assim seria impossível ter certeza de que os dados apresentados não foram manipulados e o programa perderia completamente seu sentido.

**O que está pronto:** Nada está pronto. Eu tenho pouco conhecimento em processamento de uma grande quantidade de dados estou pesquisando extensivamente os melhores algoritmos e como executá-los. Conforme o projeto for avançando, atualizarei essa sessão com uma lista do que foi feito e o que falta fazer.

**Como contribuir:** Garfe o repositório, entre em contato via [e-mail][mail], mande um sinal de fumaça. Para que tudo dê certo precisaremos de uma base sólida de matemática (estatística e probabilidade), uma programação limpa e possíveis interfaces gráficas. Preciso pensar também em qual seria o melhor canal de comunicação para trocar ideias. Se fórum no Google Groups, outro tipo de mailing list, IRC... sugestões?

Se achou o projeto interessante, me conte. Vamos conversar e fazer ele acontecer.

[foss]: http://www.gnu.org/philosophy/free-sw.html
[mine]: http://en.wikipedia.org/wiki/Text_mining
[abst]: http://en.wikipedia.org/wiki/Sentiment_analysis 
[pyth]: http://www.python.org/download/releases/2.7.5/
[para]: http://pt.wikipedia.org/wiki/Computa%C3%A7%C3%A3o_paralela
[octo]: https://code.google.com/p/octopy/
[baye]: http://en.wikipedia.org/wiki/Naive_Bayes_classifier
[tfid]: http://en.wikipedia.org/wiki/TF_IDF
[mong]: http://www.mongodb.org/
[json]: http://www.json.org/
[gpl3]: http://gplv3.fsf.org/
[mail]: mailto:contato@bbenatti.com.br
