				"type": "object",
				"properties": {
					"amount": {
						"type": "number",
						"default": "0.0"
					},
					"currency": {
						"type": "string",
						"enum": [
							"USD",
							"CAD",
							"EUR"
						]
					}
				},
				"required": [
					"amount",
					"currency"
				]
			},
			"editPrice": {
				"title": "EditPrice",
				"type": "object",
				"properties": {
					"amount": {
						"type": "number",
						"default": "0.0"
					},
					"currency": {
						"readonly": true,
						"type": "string",
						"enum": [
							"USD",
							"CAD",
							"EUR"
						]
					}
				},
				"required": [
					"amount"
				]
			}
		},
		"properties": {
			"name": {
				"type": "string",
				"pattern": "[a-z,A-Z]"
			},
			"sku": {
				"type": "string"
			},
			"createdDate": {
				"type": "string",
				"readonly": true
			}
		},
		"required": [
			"name",
			"sku"
		]
	}
}

```
