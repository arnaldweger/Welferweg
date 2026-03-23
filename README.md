# 🏥 Helferweg — Sistema de Gestão Hospitalar

> Sistema web multi-módulo desenvolvido em Python/Streamlit para automação de processos financeiros, de planejamento e controle de materiais no setor hospitalar.
> Desenvolvido de forma independente e atualmente em produção.

---

## 🎯 Contexto e motivação

Atuando no setor de planejamento e tesouraria de uma rede hospitalar de grande porte, identifiquei que diversas operações críticas eram realizadas de forma manual: conciliação de cartões, geração de pedidos, controle de OPME e monitoramento de estoque.

O **Helferweg** nasceu para centralizar e automatizar essas operações em uma única plataforma web, acessível por qualquer navegador, sem necessidade de instalação.

---

## 🗂️ Módulos em produção

### 🏦 Tesouraria
| Funcionalidade | Descrição |
|---|---|
| Painel | Visão consolidada das operações financeiras do dia |
| Conciliação Caixa | Conferência de valores de caixa com lançamentos no ERP |
| Conciliação Cartões | Cruzamento automático entre extratos de cartão e ERP Tasy |

### 📋 Planejamento
| Funcionalidade | Descrição |
|---|---|
| Agrupar Dados | Consolidação de dados de múltiplas fontes para análise |
| Top 20 | Identificação dos itens de maior impacto financeiro/operacional |
| SND | Controle de itens com necessidade de reposição |

### 🛒 Compras
| Funcionalidade | Descrição |
|---|---|
| Pedidos | Geração de pedidos em massa via integração CSV com GTPlan |
| Fornecedores | Gestão de pendências e follow-up automático por e-mail |

### 🔬 OPME
| Funcionalidade | Descrição |
|---|---|
| Arquivos | Gestão de documentos e registros de materiais especiais |
| Verificação de Materiais | Conferência e validação de itens de alto custo |

---

## 🛠️ Stack técnica

| Tecnologia | Uso |
|---|---|
| Python 3.x | Linguagem principal |
| Streamlit | Interface web multi-página |
| Pandas | Leitura, tratamento e cruzamento de dados |
| Plotly | Gráficos e dashboards interativos |
| OpenPyXL | Leitura e escrita de arquivos Excel |
| CSV / XLSX | Integração com sistemas ERP e GTPlan |
| Render | Hospedagem em nuvem (produção) |
| Git | Versionamento |

---

## 🚀 Arquitetura

```
helferweg/
├── app.py                        # Ponto de entrada — roteamento de páginas
├── components/
│   └── sidebar.py                # Menu lateral de navegação
├── pages/
│   ├── tesouraria/
│   │   ├── painel.py
│   │   ├── conferencia_caixa.py
│   │   └── conciliacao_cartoes.py
│   ├── planejamento/
│   │   ├── agrupar.py
│   │   ├── top20.py
│   │   └── snd.py
│   ├── compras/
│   │   ├── pedidos.py
│   │   └── fornecedores.py
│   ├── opme/
│   │   ├── arquivos.py
│   │   └── verificacao_materiais.py
│   └── extra/
│       └── porcentagem.py
├── requirements.txt
└── README.md
```

---

## 💡 Resultados gerados

- **Conciliação de cartões**: processo que era 100% manual passou a ser executado em segundos, com relatório de divergências gerado automaticamente
- **Pedidos em massa**: consolidação de 20–50 pedidos semanais em um único ciclo mensal com entregas semanais — redução expressiva de carga operacional
- **Follow-up de fornecedores**: e-mails de cobrança enviados automaticamente, eliminando controle manual de pendências
- **Top 20 e SND**: visibilidade imediata sobre itens críticos, antes obtida apenas com cruzamento manual de planilhas

---

## 📌 Observações

> ⚠️ Repositório privado — sistema desenvolvido de forma independente para uso interno. O código não é divulgado publicamente por conter lógicas e integrações específicas do ambiente hospitalar.

> Para demonstração em processos seletivos, estou disponível para apresentar o sistema em funcionamento com dados fictícios.

---

## 📬 Contato

**Arnald Weger**
🔗 [LinkedIn](https://www.linkedin.com/in/arnaldweger/)
📧 arnaldweger@gmail.com
📍 São Paulo, SP — Disponível para trabalho remoto
