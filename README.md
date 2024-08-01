<!--[![Google ML](https://developers.google.com/static/ml-kit/images/homepage/hero.png?width=24)](https://developers.google.com/ml-kit?hl=pt-br)[![Firebase](https://www.google.com/url?sa=i&url=https%3A%2F%2Fcommons.wikimedia.org%2Fwiki%2FFile%3AFirebase_icon.svg&psig=AOvVaw3_eY3-yB7dzBsCk1RfI3lj&ust=1710521554157000&source=images&cd=vfe&opi=89978449&ved=0CBEQjRxqFwoTCOCCwcSb9IQDFQAAAAAdAAAAABAD)](https://firebase.com)-->
# Omie app

Aguarde o vídeo abaixo carregar (acredite, há um vídeo) ou <a href="http://www.youtube.com/watch?feature=player_embedded&v=GbB4gaQxlBw" target="_blank">ou clique aqui</a> para abrir no youtube.<br/><br/>
[<img src="https://github.com/diogoroos/diogoroos/assets/78812662/cf00cf0d-6404-4581-a103-a016548d2806" heigth="300" width="300px">](https://www.youtube.com/watch?v=uyCk2mHocgQ)

## Recursos:
- O app se integra com as APIs (REST) do ERP.<br/>
- Além dos dashboards de todos os módulos, existem as seguintes funcionalidades:<br/>
  - inserir fornecedor (PF ou PJ)<br/>
  - inserir conta a pagar através de leitura de código de barras, digitação manual ou digitação do código de barras<br/>
  - consultar estoque via leitura de código de barras/QrCode ou digitação de parte (nome ou código) do produto, o que abre a tela de pesquisa<br/>
  - consulta de restrição de CPF/CNPJ<br/><br/>
Haviam outras funcionalidades que desenvolvi (calendário do CRM, inserção de tarefas no CRM, Kanban de arrastar-soltar pedido para faturar), mas não permitiram a publicação, liberando inicialmente apenas os dashboards. Apenas as 4 funcionalidades acima foram publicadas posteriormente, e as demais não liberaram até minha saída da Omie.

## Tempo:
Desenvolvi o UI no Figma entre 2-3 meses.<br/>
Depois disso desenvolvi a primeira versão com mais 3-4 meses com as funcionalidades acima (exceto consulta de restrição que só veio depois).

## Estrutura:
Nesse projeto eu fui o Dev, UX (Figma), PO e QA =D<br/>
Github e issues para controlar os cards<br/>
SCRUM<br/>

## Arquitetura:
Flutter 3.12<br/>
MVVM<br/>
Princípios S.O.L.I.D<br/>
Clean Code<br/>

## Principais bibliotecas:
Mobx para gerenciamento de estado<br/>
Modular para injeção de dependência<br/>
Firebase analytics, crashlytics, messaging, remote_config<br/>
dio para comunicação com APIs
onesignal para integração com push<br/>
google_ml_kit para leitura leitura de qrcode/barcode para consultar estoque e conta a pagar<br/>
fl_chart para gerar gráfico financeiro (o gráfico de funil foi feito na mão)<br/>
intercom para acesso ao chat com suporte<br/>
new_face_liveness (lib da CAF para face match / face authenticator)<br/>
e alguns outros com pinput, share_plus...<br/>
