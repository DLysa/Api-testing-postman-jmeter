# 🚀 API Testing Demo – Postman & JMeter

> Projekt testowania REST API z użyciem **Postman**, **JMeter** i **Swagger** na przykładzie serwisu [Reqres.in](https://reqres.in).

---

## 📦 Zawartość projektu

- 🔧 **Postman** – kolekcja testów REST API
- 📊 **JMeter** – test obciążeniowy
- 📚 **Swagger (OpenAPI)** – dokumentacja API

---

## 🧪 Postman

**Lokalizacja plików:**  
`postman/api_test_collection.json`  
`postman/environment.json`

### ✅ Jak uruchomić testy:

1. Zaimportuj kolekcję i środowisko do Postmana.
2. Wybierz środowisko.
3. Uruchom kolekcję testów (np. przez Collection Runner).

**Sprawdzane w testach:**
- Kody odpowiedzi: `200`, `201`, `204`
- Struktura odpowiedzi JSON
- Wartości pól
- Operacje na zmiennych środowiskowych

---

## ⚙️ JMeter

**Plik testowy:**  
`jmeter/load_test_plan.jmx`

### 🔁 Jak uruchomić test obciążeniowy:

1. Otwórz plik w Apache JMeter.
2. Uruchom test (▶ Start).
3. Sprawdź wyniki w „View Results Tree”.

**Parametry domyślne:**
- Liczba wątków (users): `5`
- Iteracje: `10`
- Ramp-up time: `5s`

**Sprawdzane:**
- Statusy HTTP: `200`, `201`
- Dane w odpowiedzi: `"page": 2`, `"id"`

---

## 📘 Swagger / OpenAPI

**Plik:**  
`docs/api_spec_swagger.yaml`

Możesz otworzyć plik w narzędziu takim jak [Swagger Editor](https://editor.swagger.io/) lub zaimportować do Postmana.

---

## 🛠 Technologie

- [Postman](https://www.postman.com/)
- [Apache JMeter](https://jmeter.apache.org/)
- [Swagger / OpenAPI 3.0](https://swagger.io/)
- REST API – [Reqres.in](https://reqres.in)

---