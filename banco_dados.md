

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

---
# $`\mathbb{BANCO \space DE \space DADOS}`$
---

![Static Badge](https://img.shields.io/badge/Banco%20de%20dados-N%C3%A3o_Relacional-red)

![Static Badge](https://img.shields.io/badge/Tecnologia%3A-gray)
![MongoDB](https://img.shields.io/badge/MongoDB-%234ea94b.svg?&logo=mongodb&logoColor=white)

---

### $`\sf Estrutura \space do \space banco \space em \space JSON`$

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

---

### $`\sf Diagrama \space do \space Banco \space de \space Dados`$

- Diagrama pode ser visualizado com o código JSON no site [JSON CRACK](https://jsoncrack.com/editor)

![PDF_DataModel](uploads/Database.png)
