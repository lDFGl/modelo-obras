# Auditoria Interna – Checklist de Medição de Obra

Aplicação web demonstrativa para registro e avaliação de critérios de conformidade em contratos e boletins de medição de obras.

> **Privacidade:** os registros incluídos neste repositório são fictícios e servem apenas para demonstração. Não publique dados reais de fornecedores, contratos, obras, colaboradores, documentos ou valores confidenciais.

## Funcionalidades

- Checklist de critérios por contrato.
- Avaliação por status: implementado (IM), oportunidade de melhoria (OM), não aplicável (N/A), parcialmente implementado (PI) e não implementado (NI).
- Pesos por critério e cálculo automático do percentual de conformidade.
- Quadro geral e planos de ação.
- Exportação de relatórios em Word e PDF.
- Importação e exportação de dados em JSON.
- Inclusão de evidências fotográficas.
- Armazenamento local no navegador (LocalStorage).

## Como executar

Não há etapa de compilação. Com Node.js instalado:

```bash
npm install
npm start
```

A aplicação será servida localmente pelo pacote `serve` (normalmente em http://localhost:3000).

## Estrutura atual

```text
/
├── index.html
├── package.json
├── README.md
└── www/
    ├── index.html       # interface, estilos e lógica da aplicação
    └── data/
        ├── criteria.json
        └── seed.json    # dados fictícios para demonstração
```

A lógica e a interface estão concentradas em `www/index.html`. Os arquivos JSON em `www/data` são dados de referência; alterações neles não necessariamente alteram os critérios ou os dados iniciais definidos no código da aplicação.

## Privacidade e armazenamento

- Os dados preenchidos pelo usuário ficam no armazenamento local do navegador utilizado.
- A exportação JSON pode conter fornecedores, contratos, valores, observações e imagens informados pelo usuário. Trate os arquivos exportados como documentos potencialmente confidenciais.
- Antes de compartilhar relatórios ou arquivos JSON, revise e remova informações pessoais, comerciais e operacionais.
- Não utilize este repositório público para armazenar dados reais de auditoria.
- A substituição dos arquivos na branch atual não remove dados de commits antigos. Para eliminar versões históricas expostas, é necessário reescrever o histórico do Git e verificar forks, clones e caches.

## Tecnologias

- HTML5, CSS3 e JavaScript puro.
- jsPDF e jsPDF-AutoTable para PDF.
- docx para geração de documentos Word.
- LocalStorage para persistência local.

## Observação técnica

O projeto é estático e não possui backend ou autenticação. O LocalStorage não sincroniza dados entre dispositivos e não deve ser considerado um repositório corporativo seguro.

## Licença

MIT
