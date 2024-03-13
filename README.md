# Omie app

Aguarde o vídeo abaixo carregar (acredite, há um vídeo) ou <a href="http://www.youtube.com/watch?feature=player_embedded&v=GbB4gaQxlBw" target="_blank">ou clique aqui</a> para abrir no youtube.<br/><br/>
[<img src="https://github.com/diogoroos/omie_app/assets/78812662/80126a86-93bc-43e1-8433-1bc116004331" heigth="300" width="300px">](https://www.youtube.com/watch?v=uyCk2mHocgQ)

## Recursos:
O app se integra com as APIs (REST) do ERP.<br/>
Além dos dashboards, tem as seguintes funcionalidades:<br/>
- inserir fornecedor (PF ou PJ)<br/>
- inserir conta a pagar através de leitura de código de barras, digitação manual ou digitação do código de barras<br/>
- consultar estoque via leitura de código de barras/QrCode ou digitação de parte (nome ou código) do produto, o que abre a tela de pesquisa<br/>
- consulta de restrição de CPF/CNPJ<br/><br/>
Haviam outras funcionalidades que desenvolvi (calendário do CRM, inserção de tarefas no CRM, Kanban de arrastar-soltar pedido para faturar), mas não permitiram a publicação, liberando inicialmente apenas os dashboards. Apenas as 4 funcionalidades acima foram publicadas posteriormente.

## Tempo:
Desenvolvi o UI no Figma entre 2-3 meses.<br/>
Depois disso desenvolvi a primeira versão com mais 3-4 meses com as funcionalidades acima (exceto consulta de restrição e não tão elaboradas quanto a versão que foi publicada).

## Estrutura:
Nesse projeto eu fui o Dev, UX (Figma), PO e QA =D<br/>
GIT (issues para controlar os cards), SCRUM

## Arquitetura:
Flutter 3.12<br/>
MVC + repository<br/>
Princípios S.O.L.I.D<br/>
Clean Code<br/><br/>

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
