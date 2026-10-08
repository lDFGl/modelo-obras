# Auditoria Interna – Checklist de Medição de Obra

Sistema de checklist para auditoria interna, voltado à verificação de contratos e dados para a auditoria de obras.

## 📋 O que é

Aplicação web para registrar e auditar 9 critérios de conformidade em contratos de medição de obras:
- Cadastro e vigência no ERP
- Formalização de adendos
- Valor contratual
- Planilhas de controle gerencial
- Assinatura de documentos
- Divergências monetárias
- Quadro de concorrência
- Análise fiscal (alerta)
- Documentação trabalhista (alerta)

## 🚀 Quick Start

```bash
# Instalar dependências
npm install

# Iniciar servidor de desenvolvimento
npm start

# A aplicação fica disponível em http://localhost:3000
```

## 📁 Estrutura de Pastas

```text
www/
├── index.html
├── css/
│   └── styles.css
├── data/
│   ├── criteria.json
│   └── seed.json
├── js/
│   └── app.js
└── assets/
    └── logo.png
package.json
README.md
```

## 🎯 Funcionalidades

- Checklist de critérios por contrato
- Quadro geral com indicadores de conformidade
- Exportação de relatório em Word e PDF
- Importação/exportação de dados em JSON
- Anexos fotográficos
- Plano de ação por setor
- Tema claro/escuro

## 💻 Stack

- Frontend: HTML5 + Vanilla JavaScript + CSS3
- Exportação: jsPDF + jspdf-autotable (PDF), docx (Word)
- Armazenamento: LocalStorage
- Build: estático, sem compilação

## 📝 Licença

MIT
