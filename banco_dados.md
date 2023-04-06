|[Home](home)|[Sprints](sprints)|[Requisitos](requisitos)|[Arquitetura](arquitetura)|[Processos](processos)|[Configuração](configuracao)|[Mockups](mockups)|[Banco de Dados](Banco-Dados)|[Instalação](instalacao)|[Gerência de Projeto](Gerenciamento do Projeto)|[Horários Disponiveis](horarios)|
|---|---|---|---|---|---|---|---|---|---|---|

---
# $`\mathbb{BANCO \space DE \space DADOS}`$
---

- Nosso banco de dados será não-relacional utilizando a tecnologia MongoDB

TBD (Explicação do banco de dados)

---

### Estrutura do banco em JSON

```json
{
  "veiculo": {
    "desc_cat": "string",
    "renavam_desc": "string",
    "sigla": "string",
    "pacote_def_modelo": "string",
    "versao": "string",
    "ano": "string",
    "marca": "string",
    "linha": "string",
    "motor": {
      "cilindradas": "string",
      "nro_cilindradas": "string",
      "combustiveis": [
        {
          "potencia": "string",
          "tipo_combustivel": "string"
        }
      ]
    },
    "carga": "string",
    "num_passag": "string",
    "num_portas": "string",
    "num_renavam": "string",
    "status": "string",
    "pdf_names": [
      "string"
    ]
  }
}
```

