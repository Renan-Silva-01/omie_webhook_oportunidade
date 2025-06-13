# Omie Integration com Google Sheets

Este repositório contém scripts Python para integrar a API do Omie com o Google Sheets. Ele automatiza o processo de busca de informações sobre vendedores, clientes e oportunidades, atualizando planilhas de forma eficiente e gerenciando propostas comerciais.

## Funcionalidades

- **Integração com Omie**: Consulta e atualiza dados de vendedores, clientes e oportunidades a partir da API do Omie.
- **Google Sheets**: Preenche e atualiza planilhas com informações extraídas de oportunidades.
- **Criação Automática de Propostas**: Gera cópias de planilhas modelo e preenche com os dados extraídos da API do Omie.
- **Cache**: Evita duplicação de processamento armazenando as oportunidades já processadas.
- **Webhook**: Configuração de webhook para interagir com a API do Omie e outros sistemas, acionando ações automáticas.

## Requisitos

- **Python 3.x**

### Bibliotecas

- `import os`
- `import json`
- `import requests`
- `import re`
- `from flask import Flask, request, jsonify, send_from_directory`
- `from datetime import datetime`
- `from google.oauth2 import service_account`
- `from googleapiclient.discovery import build`
- `import socket`
- `import re`
