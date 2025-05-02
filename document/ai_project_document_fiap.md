
<img src="../assets/logo-fiap.png" alt="FIAP - Faculdade de Informática e Admnistração Paulista" border="0" width=30% height=30%>

# AI Project Document - Módulo 1 - FIAP

**_Os trechos em itálico servem apenas como guia para o preenchimento da seção. Por esse motivo, não devem fazer parte da documentação final_**

## Nome do Grupo

#### Nomes dos integrantes do grupo



## Sumário

[1. Justificativa do Problema](#c1)

[2. Descrição da Solução Proposta](#c2)

[3. Tecnologias Propostas](#c3)

[4. Pipeline de Dados](#c4)

[5. Diferencial com IA Integrada e Comunicação Inteligente](#c5)

[6. Infraestrutura de Execução](#c6)

[7. Plano Inicial de Desenvolvimento](#c7)

[8. Referências](#c8)

[Anexos](#c9)

<br>

# <a name="c1"></a>1. Justificativa do Problema

*Indústrias frequentemente enfrentam paradas inesperadas nas linhas de produção, gerando perdas financeiras, atrasos logísticos e riscos à segurança operacional. A ausência de um sistema preditivo e em tempo real dificulta a prevenção de falhas. Nossa solução busca monitorar continuamente os equipamentos, identificar padrões de falhas e antecipar manutenções, promovendo um ambiente mais eficiente e inteligente..*

# <a name="c2"></a>2. Descrição da Solução Proposta

*Desenvolveremos uma plataforma inteligente de monitoramento industrial, integrando sensores IoT, armazenamento em nuvem, processamento com IA e dashboards interativos. O sistema será capaz de:

Coletar dados em tempo real via sensores (ESP32);

Armazenar os dados em um banco de dados na nuvem;

Aplicar algoritmos de machine learning para predição de falhas;

Notificar automaticamente os funcionários via aplicativo web/móvel com linguagem natural (NLP);

Exibir insights e relatórios em dashboards acessíveis.*

# <a name="c3"></a>3. Tecnologias Propostas


*Camada	Ferramentas / Tecnologias
Sensoriamento	ESP32 com sensores de vibração, temperatura e umidade
Transmissão	MQTT via WiFi
Armazenamento	PostgreSQL (Open Source Database) ou AWS RDS
Backend APIs	Python (Flask ou FastAPI)
IA / ML	Python (Scikit-learn, TensorFlow ou Keras)
Front-end	React ou Dash (Plotly) para dashboards
Notificações	Telegram Bot, WhatsApp Business API ou App personalizado
Infraestrutura	AWS EC2 (processamento), Lambda (eventos), S3 (logs)*

# <a name="c4"></a>4. Pipeline de Dados

*Sensores IoT (ESP32) simulam ou captam dados de:

Vibração anormal (indicador de falha mecânica);

Temperatura excessiva (indicador de superaquecimento);

Umidade (indicador de ambiente insalubre).

Transmissão dos dados via protocolo MQTT para servidor de ingestão.

API Coletar Dados armazena no banco de dados PostgreSQL hospedado em nuvem.

API Análise de Dados:

Realiza pré-processamento (normalização, remoção de ruído);

Usa modelos preditivos treinados com histórico;

Classifica anomalias e riscos de falha.

API Dashboard exibe:

Status dos sensores;

Alertas preditivos;

Relatórios de eficiência e manutenção sugerida.

Notificações automatizadas:

Funcionários são avisados por texto, áudio ou chatbot com recomendações práticas (ex: "Reduza carga da máquina 02, risco de falha em 12h").*


# <a name="c5"></a>5. Diferencial com IA Integrada e Comunicação Inteligente


*Além da predição de falhas, a IA utilizará técnicas de Processamento de Linguagem Natural (NLP) para traduzir insights técnicos em mensagens compreensíveis aos operadores, como:

"A máquina 3 apresentou aumento de vibração fora do padrão. Recomendamos inspeção preventiva nas próximas 4 horas."

Isso pode ser integrado com:

Chatbots internos (Telegram, WhatsApp, Microsoft Teams);

Notificações com áudio gerado por IA para áreas barulhentas (Text-to-Speech).*

# <a name="c6"></a>6. Infraestrutura de Execução


*Coleta local: ESP32 envia dados via MQTT.

Processamento em nuvem: AWS EC2 com Python.

Armazenamento escalável: AWS RDS (PostgreSQL) ou alternativa open-source.

Visualização: Dashboards via React, Dash ou Grafana.

Notificações: APIs de envio com IA + NLP.*


# <a name="c7"></a>7. Plano Inicial de Desenvolvimento


*Etapa	Atividade	Responsável
1	Escolha e simulação de sensores	Integrador IoT
2	Implementação das APIs em Python	Dev Backend
3	Pipeline de ingestão de dados	Dev Backend
4	Treinamento de modelo preditivo	Cientista de Dados
5	Integração com dashboards e alertas	Dev Frontend
6	Geração de mensagens com NLP	Dev IA/NLP*


# <a name="c8"></a>8. Referências

_Incluir as principais referências de seu projeto, para que outros possam consultar caso tenham interesse em aprofundar._

# <a name="c9"></a>Anexos

*Inclua aqui quaisquer complementos para seu projeto, como diagramas, imagens, tabelas etc. Organize em sub-tópicos utilizando headings menores (use ## ou ### para isso).*
