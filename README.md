## Dokumentasi API - Praktikum CRUD

Tampilan Web
<img width="1919" height="969" alt="image" src="https://github.com/user-attachments/assets/e660ba36-f417-4585-af83-07f750b756ee" />

Tampilan Database
<img width="1919" height="1019" alt="image" src="https://github.com/user-attachments/assets/90c1059c-1aac-4cd0-85d6-1b1cc85b18d6" />

### 1. Create User
**Method:** `POST`  
**Endpoint:** `/api/users`

**Request Body:**
```json
{
  "age": 25,
  "name": "Praktikum1"
}
```

**Response (201 Created):**
```json
{
  "status": "success",
  "data": {
    "age": 25,
    "id": "d1be5c98-1bef-41c5-935b-4bdaf8b0945e",
    "name": "Praktikum1"
  }
}
```
**Response (404 Not Found):**
```json
{
    "timestamp": "2026-03-04T12:10:00.364Z",
    "status": 404,
    "error": "Not Found",
    "path": "/api/user"
}
```

---

### 2. Get All Users
**Method:** `GET`  
**Endpoint:** `/api/users`

**Response (200 OK):**
```json
{
  "status": "success",
  "data": [
    {
      "age": 20,
      "id": "691a3070-405a-4862-93fc-ab11a5b12b03",
      "name": "Indra Hafid Saputra"
    }
  ]
}
```

---

### 3. Update User
**Method:** `PUT`  
**Endpoint:** `/api/users/{id}`

**Request Body:**
```json
{
  "age": 5,
  "name": "Update PRAK1"
}
```

**Response (200 OK):**
```json
{
  "status": "success",
  "data": {
    "age": 5,
    "id": "d1be5c98-1bef-41c5-935b-4bdaf8b0945e",
    "name": "Update PRAK1"
  }
}
```

---

### 4. Delete User
**Method:** `DELETE`  
**Endpoint:** `/api/users/{id}`

**Response (200 OK):**
```json
{
  "status": "success delete user with id d1be5c98-1bef-41c5-935b-4bdaf8b0945e"
}
```
