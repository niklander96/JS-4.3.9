"info": {
		"_postman_id": "a7f10271-6838-484b-aeba-efae09dc9330",
		"name": "POSTMAN ECHO",
		"schema": "https://schema.getpostman.com/json/collection/v2.1.0/collection.json",
		"_exporter_id": "23859633"
	},
	"item": [
		{
			"name": "New Request",
			"request": {
				"method": "POST",
				"header": [],
				"body": {
					"mode": "raw",
					"raw": "{\r\n  \"user\": {\r\n    \"username\": \"nekitlok\",\r\n    \"email\": \"nik.loktev151069@gmail.com\",\r\n    \"password\": \"Sopiho1410\"\r\n  }\r\n}",
					"options": {
						"raw": {
							"language": "json"
						}
					}
				},
				"url": {
					"raw": "https://blog.kata.academy/api/users",
					"protocol": "https",
					"host": [
						"blog",
						"kata",
						"academy"
					],
					"path": [
						"api",
						"users"
					]
				}
			},
			"response": []
		},
		{
			"name": "https://blog.kata.academy/api/user/login",
			"protocolProfileBehavior": {
				"disableBodyPruning": true
			},
			"request": {
				"auth": {
					"type": "bearer",
					"bearer": [
						{
							"key": "token",
							"value": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjYzNDk4M2Q5M2NmNzA1MWIwMDgyYWYxYyIsInVzZXJuYW1lIjoibmVraXRsb2siLCJleHAiOjE2NzA5NDYyNjUsImlhdCI6MTY2NTc2MjI2NX0.X-qt8UcT1a4iEOdzNHA7ngeFSbeiGD9W0WneyzV4edc",
							"type": "string"
						}
					]
				},
				"method": "GET",
				"header": [],
				"body": {
					"mode": "raw",
					"raw": "",
					"options": {
						"raw": {
							"language": "json"
						}
					}
				},
				"url": {
					"raw": "https://blog.kata.academy/api/user",
					"protocol": "https",
					"host": [
						"blog",
						"kata",
						"academy"
					],
					"path": [
						"api",
						"user"
					],
					"query": [
						{
							"key": "",
							"value": null,
							"disabled": true
						}
					]
				}
			},
			"response": []
		}
	]
}
