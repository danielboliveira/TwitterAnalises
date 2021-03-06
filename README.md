# Twitter Análises

<H3> Os resultados da análise de candidatos estarão nesse endereço: <a href='http://www.dbodata.com.br/' target='_blank'>http://www.dbodata.com.br/</a></H3>

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
        <li> <a href='https://github.com/danielboliveira/TwitterAnalises/blob/master/An%C3%A1lise%20Sentimentos%20-%2022062018.pdf'> Resultados em 22/06/2018 </a></li>
        <li> <a href='https://github.com/danielboliveira/TwitterAnalises/blob/master/Eleicoes2018/An%C3%A1lise%20Lula%20e%20Bolsanaro%2009-07-18.pdf'> Lula x Bolsonaro (09/07) - durante a manobra para soltar o Lula </a>
    </ul>
  </li>
</ol>

### Análise específica: Seleção Brasileira - Copa 2018

<p>Desenvolvi um crawler específico para atuar durante os jogos da seleção brasileira. Para verificar o comportamento dos torcedores na rede social, bem como a atuação de perfis de influência (aqui os defino como sendo perfis com muitos seguidores e que suas postagens, normalmente de cunho pejorativo, tem muita reverberação na rede).</p>

#### Brasil x Costa Rica - 22/06/2018

<img src = 'https://github.com/danielboliveira/TwitterAnalises/blob/master/Analise_Sentimento_BrasilxCostaRica_22062018.png'>

<p> O detalhamento pode ser visto <a href='https://goo.gl/upWjCE'>aqui</a> </p>

#### Dos perfis de influência durante a partida do dia 22/06

<p> Foi realizado um estudo específico para verificar a real influência de determinados perfis na rede. A capacidade de propagação de postagens. E, por extensão pode-se verificar os riscos e janelas temporais para propagação das chamadas <i>fake news</i>.</p>
<p> Os resultados da análise pode ser vistos <a href='https://github.com/danielboliveira/TwitterAnalises/blob/master/An%C3%A1lise%20de%20perfis%20de%20influ%C3%AAncia%20no%20Twitter.pdf'> aqui </a>

### Reputação Neymar
<p>Ainda usando o evento Copa do Mundo 2018 como referência para os testes da ferramenta e melhoria nos algoritmos, vou realizar um acompanhamento da reputação do Neymar próxmo dos jogos</p>
<p>Entre os dias 26/6 e 27/06 realizei a análise de reputação do Neymar no Twitter. Os resultados podem ser visto: <a href='https://github.com/danielboliveira/TwitterAnalises/blob/master/Analise%20Neymar%2026-6%20a%2027-6.pdf'> aqui </a></p>

<p><b>29/06/2018</b> - Fiz alguns ajustes nos algoritmos de identificação e classificação de termos. Abaixo seguem as nuvens de termos de maior frequência nos Posts do Neymar (não levando em conta o sentimento). A primeira Nuvem corresponde o período antes do jogo do dia 27/6 (26/06 até a madrugada do dia 27/06) e a segunda é após o jogo (das 17:00 do dia 27/06 até 01:30 do dia 28/06)</p>

<img src='https://github.com/danielboliveira/TwitterAnalises/blob/master/imagens/Analise_Cloud_Words_Neymar_26062018.png'/>
</br>
<img src='https://github.com/danielboliveira/TwitterAnalises/blob/master/imagens/Analise_Cloud_Words_Neymar_27062018.png'/>
</br>
<p><h3>Jogo 4 (02/07/2018)</h3></p>
<p>Levando-se em conta os resultados da análise do jogo 4 a rejeição ao Neymar está consolida. E, pelo visto, mesmo se o Brasil ganhar a copa não vai mudar. No entanto, o mesmo ocorre para aqueles que gostam dele.</p>
<p><a href='https://github.com/danielboliveira/TwitterAnalises/blob/master/Neymar%20Jogo%204%2002-07.pdf'>Análise de Reputação Jogo 4 </a></p>

##Fechamento da Análise da Copa
<p> Com a eliminação do Brasil da Copa de 2018, vamos as últimas análises de reputação. Como esperado a reputação do Neymar permanece ruim e deve piorar nos próximos meses. Já da seleção brasileira não ficou tão ruim assim.</p>
<ul>
  <li><a href='https://github.com/danielboliveira/TwitterAnalises/blob/master/An%C3%A1lise%20Neymar%20Jogo%205.pdf'>Reputação Neymar Jogo 5 </a></li>
  <li><a href='https://github.com/danielboliveira/TwitterAnalises/blob/master/Analise%20Sele%C3%A7%C3%A3o%20Brasileira%20Jogo%205.pdf'>Reputação Seleção Brasileira Jogo 5</a></li>
</ul>
<p>Após esse período de copa vou voltar analisar nossos políticos para a corrida presidencial!</p>
