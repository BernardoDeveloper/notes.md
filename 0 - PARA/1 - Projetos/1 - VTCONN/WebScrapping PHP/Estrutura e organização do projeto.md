Source: Mentalidade - brainstorm
Related: [[WebScrapping Wagner PHP]]

---

Quais os dados que eu preciso entregar na tabela:
1. Informações do produto (código do produto, descrição, preço ...)
2. Código ofical da operação CFOP
3. Dados da nota fiscal

Onde eu tenho que buscar para conseguir cada dado:
1. Na url `https://bling.com.br/Api/v3/produtos` é possível obter os dados dos produtos registrados no sistema
2. Código ofical da operação ??
3. Os dados da nota fiscal estão disponível em `https://bling.com.br/Api/v3/nfe` mas ele não retorna os dados de qual produto está vendendo

Ao buscar em **pedidos de vendas** os dados retornados são o seguinte:
```json
{
	"id": 19378751114,
	"numero": 8584,
	"numeroLoja": "",
	"data": "2024-12-10",
	"dataSaida": "2024-12-10",
	"dataPrevista": "2024-12-10",
	"totalProdutos": 89550,
	"total": 89550,
	"contato": {
		"id": 15899619305,
		"nome": "GEOLAB INDUSTRIA FARMACEUTICA",
		"tipoPessoa": "J",
		"numeroDocumento": "03.485.572/0001-04"
	},
	"situacao": {
		"id": 6,
		"valor": 0
	},
	"loja": {
		"id": 0
	}
},
```

