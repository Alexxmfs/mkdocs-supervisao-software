# Testes da API - Pytest

Para validar a API do projeto, foi desenvolvido um script em Pytest para verificar as funcionalidades básicas de criação e listagem de registros.

```python
import requests

API_URL = "http://127.0.0.1:3000"  

def test_post():
    data = {
        "nome": "Maria Souza",
        "email": "maria.souza@example.com"
    }

    response = requests.post(f"{API_URL}/criar", json=data)

    assert response.status_code == 201, f"Unexpected status code: {response.status_code}"
    assert response.text == '', "Erro inesperado ao criar registro"

def test_get():
    response = requests.get(f"{API_URL}/listar")

    assert response.status_code == 200, f"Unexpected status code: {response.status_code}"
    try:
        response_json = response.json()
    except ValueError as e:
        assert False, f"Falha ao decodificar JSON: {e}"

    assert isinstance(response_json, list), f"Esperado uma lista, mas recebeu: {type(response_json)}"
    assert len(response_json) > 0, "A lista retornada está vazia"
