## Dokumentasi API - Praktikum CRUD

Tampilan Web
<img width="1919" height="968" alt="image" src="https://github.com/user-attachments/assets/b7a2d730-5f92-46ab-ac00-c0c7af5d0f34" />


Tampilan Database
<img width="1919" height="1020" alt="image" src="https://github.com/user-attachments/assets/b4208932-11de-44ce-b01d-929eff678255" />


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
    "id": "841d3394-7810-46ff-bdb2-da4035e0fc74",
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
    },
    {
      "age": 25,
      "id": "841d3394-7810-46ff-bdb2-da4035e0fc74",
      "name": "Update PRAK1"
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
  "age": 25,
  "name": "Update PRAK1"
}
```

**Response (200 OK):**
```json
{
  "status": "success",
  "data": {
    "age": 25,
    "id": "841d3394-7810-46ff-bdb2-da4035e0fc74",
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
    "status": "success delete user with id 841d3394-7810-46ff-bdb2-da4035e0fc74"
}
```
