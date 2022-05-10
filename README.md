<h1> Challenge_DataScience </h1>
<img src="https://user-images.githubusercontent.com/73675930/167624754-ea3dfad0-6dd3-4830-8a10-53ba329832b7.png"/>


**Em desenvolvimento**

<h2>Projeto Predição de Churn | Alura Voz</h2>
<h3>Contextualização e Objetivo</h3>

<ul>
  <p>A operadora de telecomunicações Alura Voz necessita de uma análise para a área de vendas da empresa, com o objetivo de reduzir a Taxa de Evasão de Clientes, conhecido como Churn Rate (taxa de saída dos clientes). Basicamente, o Churn Rate indica o quanto a empresa perdeu de receita ou clientes em um período de tempo.

Inicialmente é necessário fazer a idenficação de clientes que teriam uma maior chance de deixar a empresa investigando algumas características de clientes ou dos planos de clientes para tentar classificar estas pessoas como potenciais candidatas a deixar a empresa ou não.</p>
</ul>

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
<h3>Etapas | Resumo</h3>
