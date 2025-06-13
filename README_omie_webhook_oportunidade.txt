Omie Integration with Google Sheets
Este repositório contém scripts Python para integrar a API do Omie com o Google Sheets. Ele automatiza o processo de busca de informações de vendedores, clientes e oportunidades, atualizando planilhas de forma eficiente e gerenciando propostas comerciais.

Funcionalidades
Integração com Omie: Consulta e atualiza dados de vendedores, clientes e oportunidades.

Google Sheets: Preenche e atualiza planilhas com informações de oportunidades.

Criação Automática de Propostas: Gera cópias de planilhas modelo e preenche com os dados extraídos.

Cache: Evita duplicação de processamento ao armazenar oportunidades já processadas.

Webhook: Configuração de webhook para interagir com a API Omie e outros sistemas.

Requisitos
Python 3.x

Bibliotecas:

requests

google-api-python-client

google-auth

google-auth-httplib2

google-auth-oauthlib

flask

Instale as dependências com:

Copiar
Editar
pip install -r requirements.txt
Configuração
Credenciais do Omie:

Gere sua OMIE_APP_KEY e OMIE_APP_SECRET no Omie.

Credenciais Google API:

Crie um projeto no Google Cloud Console.

Ative as APIs do Google Sheets e Google Drive.

Baixe as credenciais em formato JSON e salve como google_creds.json.

Configuração no Código:

Substitua as variáveis OMIE_APP_KEY, OMIE_APP_SECRET, e GOOGLE_CREDS_FILE com os valores correspondentes.

Como Usar
Iniciar o Servidor Flask:

Copiar
Editar
python app.py
Integração:

O servidor estará disponível e pronto para receber notificações e realizar atualizações nas planilhas automaticamente.

Exemplo de Uso
O script irá automaticamente preencher as informações de oportunidade, cliente, contato e vendedor na planilha do Google, além de gerar a proposta com um número sequencial.

Licença
Este projeto está licenciado sob a MIT License.
