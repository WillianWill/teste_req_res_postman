{
	"info": {
		"_postman_id": "6d79e227-cd25-4723-9e26-9b3d7c07fa97",
		"name": "TESTE_REQ_RES",
		"schema": "https://schema.getpostman.com/json/collection/v2.1.0/collection.json"
	},
	"item": [
		{
			"name": "Validar email por ID",
			"event": [
				{
					"listen": "test",
					"script": {
						"exec": [
							"pm.test(\"Validar status code\", function () {\r",
							"    pm.response.to.have.status(200);\r",
							"});\r",
							"\r",
							"\r",
							"pm.test(\"Validar email id 7\", function () {\r",
							"    pm.expect(pm.response.text()).to.include(email);\r",
							"});"
						],
						"type": "text/javascript"
					}
				},
				{
					"listen": "prerequest",
					"script": {
						"exec": [
							"const email = \"michael.lawson@reqres.in\""
						],
						"type": "text/javascript"
					}
				}
			],
			"request": {
				"method": "GET",
				"header": [],
				"url": {
					"raw": "{{base_url}}users?page=2&id=7",
					"host": [
						"{{base_url}}users"
					],
					"query": [
						{
							"key": "page",
							"value": "2"
						},
						{
							"key": "id",
							"value": "7"
						}
					]
				}
			},
			"response": []
		},
		{
			"name": "{{base_url}}users",
			"event": [
				{
					"listen": "test",
					"script": {
						"exec": [
							"let nome = \"teste cadastrar\"\r",
							"let job = \"QA\"\r",
							"\r",
							"pm.test(\"Validar se dados cadastrados\", function () {\r",
							"    pm.expect(pm.response.text()).to.include(nome);\r",
							"     pm.expect(pm.response.text()).to.include(job);\r",
							"});\r",
							"\r",
							"pm.test(\"Validar status code 201\", function () {\r",
							"    pm.response.to.have.status(201);\r",
							"});"
						],
						"type": "text/javascript"
					}
				}
			],
			"request": {
				"method": "POST",
				"header": [],
				"body": {
					"mode": "raw",
					"raw": "{\r\n    \"name\": \"teste cadastrar\",\r\n    \"job\": \"QA\"\r\n}",
					"options": {
						"raw": {
							"language": "json"
						}
					}
				},
				"url": {
					"raw": "{{base_url}}users",
					"host": [
						"{{base_url}}users"
					]
				}
			},
			"response": []
		}
	]
}