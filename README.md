{
	"info": {
		"_postman_id": "a7f10271-6838-484b-aeba-efae09dc9330",
		"name": "POSTMAN ECHO",
		"schema": "https://schema.getpostman.com/json/collection/v2.1.0/collection.json",
		"_exporter_id": "23859633"
	},
	"item": [
		{
			"name": "register",
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
			"name": "auth",
			"request": {
				"method": "POST",
				"header": [],
				"body": {
					"mode": "raw",
					"raw": "{\r\n  \"user\": {\r\n    \"email\": \"nik.loktev151069@gmail.com\",\r\n    \"password\": \"Sopiho1410\"\r\n  }\r\n}",
					"options": {
						"raw": {
							"language": "json"
						}
					}
				},
				"url": {
					"raw": "https://blog.kata.academy/api/users/login",
					"protocol": "https",
					"host": [
						"blog",
						"kata",
						"academy"
					],
					"path": [
						"api",
						"users",
						"login"
					]
				}
			},
			"response": []
		},
		{
			"name": "GetCurrentUser",
			"protocolProfileBehavior": {
				"disableBodyPruning": true
			},
			"request": {
				"auth": {
					"type": "bearer",
					"bearer": [
						{
							"key": "token",
							"value": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjYzNDk4M2Q5M2NmNzA1MWIwMDgyYWYxYyIsInVzZXJuYW1lIjoibmVraXRsb2siLCJleHAiOjE2NzA5NTA3ODUsImlhdCI6MTY2NTc2Njc4NX0.3LpYoEKQsjV-qcFwmFzBfIGkyITUPPAKmy-eIRHdr_g",
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
