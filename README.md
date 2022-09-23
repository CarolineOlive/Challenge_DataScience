<h1> Challenge_DataScience </h1>

<h2>Projeto Predição de Churn | Alura Voz</h2>
  O projeto foi desenvolvido utilizando <b>linguagem Python</b> no jupyter notebook do Google Colab. O python possui um série de bibliotecas que nos auxiliam na construção das análises e modelagem dos dados. Neste projeto, foram utilizadas as seguintes:
<li>pandas
<li> pandas profiling (gera um relatório interativo - ProfileReport - com análise exploratória dos dados, tipos de variáveis, alertas de correlação e dependência, entre outras informações)
<li>numpy
<li>matplotlib
<li>seaborn
<li>scikit-learn
<li>imbalanced-learn
<p>

| :placard: Vitrine.Dev |     |
| -------------  | --- |
| :sparkles: Nome        | <b>Projeto Predição de Churn | Alura Voz</b>
| :label: Tecnologias | python, pandas, pandas profililing, sklearn, imbalanced-learn
| :rocket: URL         | https://github.com/CarolineOlive/Challenge_DataScience
| :fire: Desafio     | 

<!-- Inserir imagem com a #vitrinedev ao final do link -->
![projeto_final_challenge1](https://user-images.githubusercontent.com/73675930/167624754-ea3dfad0-6dd3-4830-8a10-53ba329832b7.png#vitrinedev)

  
<h3>Contextualização</h3>

<ul>
  <p>A operadora de telecomunicações Alura Voz necessita de uma análise para a área de vendas da empresa, com o objetivo de reduzir a Taxa de Evasão de Clientes, conhecido como Churn Rate (taxa de saída dos clientes). Basicamente, o Churn Rate indica o quanto a empresa perdeu de receita ou clientes em um período de tempo.
    
. : O github não suporta o relatótio interativo carregado diretamente no notebook. Por isso os relatório foram salvos em formato .html e disponibilizados em uma <a href="https://drive.google.com/drive/folders/1ZiKZCsZjAC0asDXatkhpay5vlQ68CeUG?usp=sharing">pasta no drive</a>.
</ul>

<h3>Objetivo</h3>
<ul>
  <p>Identificar clientes que teriam uma maior chance de deixar a empresa investigando algumas características de clientes e/ou dos planos por eles adquiridos.</p>
</ul>
   
<h3>Conclusão</h3>
<ul>
  <p>Em uma perspectiva de retenção de clientes, é interessante conseguir prever aqueles com maior potencial de evasão. Sendo assim, o melhor modelo é aquele que possui maior taxa de acerto para churn (True positive ou verdadeiro positivo). Isso se deve ao fato de que, da perspectiva de negócio, é mais fácil e mais barato manter um cliente do que conseguir novos clientes.

  Sendo assim, optei por dar maior peso, ou seja, considerar como melhor modelo, aquele que retornou a menor quantidade de falsos negativos, modelo <font color ='#1e2f4d'><b>Decision Tree Classifier</b></font>.

  O modelo foi testado com a base de dados balanceado utilizando 3 abordagens, over-sampling, under-sampling e SMOTE. 

  A melhor performance se deu aplicando o SMOTE. Apesar do valor baixo para a precisão da variável 1 (churn), o recall melhorou muito, comparado com o resultado obtido com a base sem balanceamento, apresentando o menor número de falsos-positivos dentre as abordagens de balanceamento dos dados e redução dos falsos-negativos.

  Adicionalmente, optei por teste o modelo com os dados de clientes que estavam sem informações de churn na base de dados, fornecendo um lista de cliente e suas probabilidades de churn.

  Aplicando o modelo, 88 cliente foram classificados como churn e 136 como não prováveis de churn. A lista de clientes e probabilidades de churn foi disponibilizada para a empresa.</p>
</ul>

<h3>Etapas | Resumo</h3>
  <p> infográfico em desenvolvimento</p>

    
_____


<h4>Dados</h4>
<ul>
  <p>O conjunto de dados disponibilizado via API foi tratado com foco na otimização de cada um dos modelos com a finalidade de obter o melhor resultado para a tomada de decisão da Alura Voz.

dados: https://raw.githubusercontent.com/sthemonica/alura-voz/main/Dados/Telco-Customer-Churn.json

Uma forma de pré-visualizar os dados contidos em uma json é utilizar a ferramenta online <a href="https://codebeautify.org/jsonviewer">Code Beautify</a>. Por meio dela é possível visualizar os níveis contidos no JSON.

A base de dados possui o número de identificação do cliente e se o cliente deixou ou não a empresa, e ainda, informações sobre:


<b>Cliente:</b>
<ul>
  <li>gender: gênero (masculino e feminino)
 <li>SeniorCitizen: informação sobre um cliente ter ou não idade igual ou maior que 65 anos
 <li>Partner: se o cliente possui ou não um parceiro ou parceira
 <li>Dependents: se o cliente possui ou não dependentes
</ul>
<b>Serviço de telefonia</b>
<ul>
 <li>tenure: meses de contrato do cliente
 <li>PhoneService: assinatura de serviço telefônico
 <li>MultipleLines: assisnatura de mais de uma linha de telefone
</ul>
<b>Serviço de internet</b>
<ul>
 <li>InternetService: assinatura de um provedor internet
 <li>OnlineSecurity: assinatura adicional de segurança online
 <li>OnlineBackup: assinatura adicional de backup online
 <li>DeviceProtection: assinatura adicional de proteção no dispositivo
 <li>TechSupport: assinatura adicional de suporte técnico, menos tempo de espera
  <li>StreamingTV: assinatura de TV a cabo
  <li>StreamingMovies: assinatura de streaming de filmes
</ul>
<b>Contrato</b>
<ul>
  <li>Contract: tipo de contrato
  <li>PaperlessBilling: se o cliente prefere receber online a fatura
  <li>PaymentMethod: forma de pagamento
  <li>Charges.Monthly: total de todos os serviços do cliente por mês
  <li>Charges.Total: total gasto pelo cliente
  </ul>
</ul>
