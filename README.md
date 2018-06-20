# Twitter Análises

<p>
Nesse repositório encontra-se resultados de análises realizadas em post e usuários do Twitter. A motivação desses trabalhos foi a minha ampliação de conhecimentos em python, aplicação e novas tecnologias de Ciência de Dados (machine learning, PLN e outras).
</p>
<p>
Os dados foram obtidos através da  <a href='https://developer.twitter.com/en/docs/tweets/timelines/api-reference/get-statuses-user_timeline.html' target= '_blank'>API do Twitter</a> - em sua versão <i>free</i>. Assim, sendo, foi construído um crawler que a cada hora capturava cerca de 1000 post por hora (limitação da API), baseando em conjunto de palavras e termos de pesquisa.
</p>
<p>
Para facilitar o processo de análise e síntese dos dados está sendo utilizando uma base em SQL Server. Uma rotina em python importar os Twittes capturados. Realizando a identificação de entidades (através de processamento de linguagens naturais - PLN), atualização de usuários (uma ML irá identificar possíveis robôs) e análise de sentimento (se o post é positivo, negativo ou neutro - também um Machine Learning é reponsável por isto)
</p>

<p>
Este trabalho tem como objetivo mostrar tendências e provar a viabilidade dessas tecnologias para uso de análise de reputação em redes, identificação de robôs e possíveis perfis utilziados para divulgação de fakenews e manipulação de opinião pública. A ideia é meramente acadêmica.
</p>

## Histórico

<ol>
  <li> Análise de sentimento
      <ul>
         <li><a href='https://github.com/danielboliveira/TwitterAnalises/blob/master/Resultados%20An%C3%A1lise%20de%20Sentimentos%20-%2020062018.pdf'> Resultados em 20/06/2018 </a></li>
    </ul>
  </li>
</ol>

