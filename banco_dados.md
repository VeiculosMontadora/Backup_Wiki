

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
  "pdf": {
    "nome": "string",
    "status": "string",
    "ultimo_visto": "Date",
    "criado": "Date",
    "veiculos": [
      {
        "desc_cat": {
          "valor": "string",
          "copiado": true
        },
        "renavam_desc": {
          "valor": "string",
          "copiado": true
        },
        "sigla": {
          "valor": "string",
          "copiado": true
        },
        "pacote_def_modelo": {
          "valor": "string",
          "copiado": true
        },
        "versao": {
          "valor": "string",
          "copiado": true
        },
        "ano": {
          "valor": "string",
          "copiado": true
        },
        "marca": {
          "valor": "string",
          "copiado": true
        },
        "linha": {
          "valor": "string",
          "copiado": true
        },
        "motor": {
          "cilindradas": {
            "valor": "string",
            "copiado": true
          },
          "nro_cilindradas": {
            "valor": "string",
            "copiado": true
          },
          "combustiveis": [
            {
              "potencia": {
                "valor": "string",
                "copiado": true
              },
              "tipo_combustivel": {
                "valor": "string",
                "copiado": true
              }
            }
          ]
        },
        "carga": {
          "valor": "string",
          "copiado": true
        },
        "num_passag": {
          "valor": "string",
          "copiado": true
        },
        "num_portas": {
          "valor": "string",
          "copiado": true
        },
        "num_renavam": {
          "valor": "string",
          "copiado": true
        }
      }
    ]
  }
}
```

### Diagrama do Banco de dados

![](https://tools.ages.pucrs.br/veiculos-via-montadora/wiki/-/raw/main/pictures/database.png)

