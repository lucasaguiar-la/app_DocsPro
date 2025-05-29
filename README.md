# DocsPro - Automação de Processamento de Documentos

## Descrição
O DocsPro é uma aplicação desktop desenvolvida em Python para automatizar o processamento, conversão e integração de documentos entre o Zoho e o sistema SIGADM. A aplicação oferece uma interface gráfica amigável para gerenciar todo o fluxo de trabalho de documentos.

## Preview
<img src="docs/Preview DocsPro.gif" alt="Preview do DocsPro" width="700"/>

> Nota: Este preview é apenas demonstrativo. O sistema real pode ter interface e funcionalidades diferentes por se tratar de uma aplicação proprietária.

Para visualização mais detalhada acesse a pasta `docs/`

## Funcionalidades Principais

### Processamento Automático
- Download automático de documentos do Zoho
- Conversão de diferentes formatos de arquivo para PDF
- Compressão de arquivos PDF grandes
- Integração automática com o SIGADM
- Atualização automática de status no Zoho

### Modos de Operação
1. **Modo Automático**: Executa todo o processo em sequência
2. **Modo Manual**: Permite executar etapas específicas:
   - Download de Documentos
   - Tratamento de Arquivos
   - Execução do SIGADM
   - Marcação de Checkboxes
   - Registro de Não Processados
   - Limpeza de Pasta

### Sistema de Login
- Interface de login segura
- Armazenamento seguro de credenciais
- Validação de autenticação

## Dependências do Sistema

### Dependências Principais
- Python 3.8+
- pymongo
- customtkinter
- aiohttp
- PyAutoGUI
- Pillow
- PyPDF2
- python-dotenv
- Ghostscript

### Bibliotecas Adicionais
```txt
pillow_heif
comtypes
psutil
pyWinActivate
```

## Estrutura do Projeto
```
DocsPro/
├── api/                 # Integrações com APIs (Zoho)
├── gui/                 # Interface gráfica
├── logs/                # Sistema de logs
├── robot/               # Automação SIGADM
├── token_data/          # Gestão de tokens
├── utils/               # Utilitários
├── workflow/            # Controlador de fluxo
└── files/              # Arquivos processados
```

## Logs e Monitoramento
- Logs detalhados de operações em `logs/log_record/`
- Registro de arquivos não processados em `logs/unprocessed_record/`
- Sistema de backup dos dados brutos originais em `original_files/`

## Segurança
- Autenticação de dois níveis (local + SIGADM)
- Tokens de API armazenados de forma segura
- Backup automático de arquivos originais

## ⚠️ Aviso Legal
Este repositório contém apenas a documentação e a estrutura básica do projeto DocsPro. O código-fonte completo é proprietário e de uso exclusivo da Guillaumon.

### Licença
Copyright © 2024 Guillaumon. Todos os direitos reservados.

Este README e a estrutura de diretórios estão disponíveis sob a licença [CC BY-NC-ND 4.0](https://creativecommons.org/licenses/by-nc-nd/4.0/):
- ✅ Você pode compartilhar e visualizar a documentação
- ❌ Não é permitido uso comercial
- ❌ Não é permitido modificar ou criar trabalhos derivados
- ℹ️ Deve dar crédito apropriado à Guillaumon

## Autores
- Lucas Aguiar - Desenvolvimento e Manutenção

---
