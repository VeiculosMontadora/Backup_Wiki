

[![](https://img.shields.io/badge/Home-000000?style=for-the-badge&logo=markdown&logoColor=white)](home)

# Documentação do negócio
[![](https://img.shields.io/badge/Sprints-000000?style=for-the-badge&logo=markdown&logoColor=white)](sprints)
[![](https://img.shields.io/badge/Requisitos-000000?style=for-the-badge&logo=markdown&logoColor=white)](requisitos)
[![](https://img.shields.io/badge/Processos-000000?style=for-the-badge&logo=markdown&logoColor=white)](processos)
[![](https://img.shields.io/badge/Gerência-000000?style=for-the-badge&logo=markdown&logoColor=white)](gerencia)
[![](https://img.shields.io/badge/Horários-000000?style=for-the-badge&logo=markdown&logoColor=white)](horarios)
[![](https://img.shields.io/badge/squads-000000?style=for-the-badge&logo=markdown&logoColor=white)](squads)

# Documentação técnica
[![](https://img.shields.io/badge/Arquitetura-000000?style=for-the-badge&logo=markdown&logoColor=white)](arquitetura)
[![](https://img.shields.io/badge/Mockups-000000?style=for-the-badge&logo=markdown&logoColor=white)](mockups)
[![](https://img.shields.io/badge/Banco_de_dados-FF7518?style=for-the-badge&logo=markdown&logoColor=black)](banco_dados)
[![](https://img.shields.io/badge/Instalação-000000?style=for-the-badge&logo=markdown&logoColor=white)](instalacao)
[![](https://img.shields.io/badge/Configuração-000000?style=for-the-badge&logo=markdown&logoColor=white)](configuracao)

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

### Diagrama do Banco de dados

![](https://tools.ages.pucrs.br/veiculos-via-montadora/wiki/-/raw/main/pictures/database.png)

