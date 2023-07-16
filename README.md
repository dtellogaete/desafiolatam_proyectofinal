# CONTRATO API REST 

## API Endpoints - Contrato de Datos

A continuación, se presenta un breve resumen del contrato de datos para cada uno de los endpoints de la API.

### POST Login

Endpoint: `/api/login`

**Request (Solicitud)**:

```json
{
  "payload": {
    "email": "string",
    "password": "string"
  }
}
```

**Response (Respuesta)**:

```json
{
  "token": "string"
}

```

**user**:

```json
{
  "id": "string",
  "email": "string",
  "name": "string",
  "lastname": "string",
  "rut": "string",
  "phone": "string",
  "address": "string",
  "city": "string",
  "region": "string",
  "telephone": "string",
  "role": "string",
  "store_name": "string",
  "store_razon": "string",
  "store_address": "string",
  "store_city": "string",
  "store_region": "string",
  "store_logo": "string"
}
```

### POST Users

Endpoint: `/api/users`

**Request (Solicitud)**:

```json
{
  "payload": {
    "email": "string",
    "password": "string",
    "name": "string",
    "lastname": "string",
    "rut": "string",
    "phone": "string",
    "address": "string",
    "city": "string",
    "region": "string",
    "telephone": "string",
    "role": "string",
    "store_name": "string",
    "store_razon": "string",
    "store_address": "string",
    "store_city": "string",
    "store_region": "string",
    "store_logo": "string"
  }
}
```

### GET User

Endpoint: `/api/user/:id`

**Request (Solicitud)**:

```json
{
  "payload": {
    "id": "integer"
  }
}
```

**Response (Respuesta)**:

```json
{
  "id": "string",
  "email": "string",
  "name": "string",
  "lastname": "string",
  "rut": "string",
  "phone": "string",
  "address": "string",
  "city": "string",
  "region": "string",
  "telephone": "string",
  "role": "string",
  "store_name": "string",
  "store_razon": "string",
  "store_address": "string",
  "store_city": "string",
  "store_region": "string",
  "store_logo": "string"
}
```

### PUT User

Endpoint: `/api/user/:id`

**Request (Solicitud)**:

```json
{
  "payload": {
    "id": "integer",
    "email": "string",
    "name": "string",
    "lastname": "string",
    "rut": "string",
    "phone": "string",
    "address": "string",
    "city": "string",
    "region": "string",
    "telephone": "string",
    "role": "string",
    "store_name": "string",
    "store_razon": "string",
    "store_address": "string",
    "store_city": "string",
    "store_region": "string",
    "store_logo": "string"
  }
}
```

## Contrato de Datos - Tabla Products

### POST Products

Endpoint: `/api/products`

**Request (Solicitud)**:

```json
{
  "payload": {
    "id_user": "integer",
    "name": "string",
    "description": "string",
    "price": "integer",
    "brand": "string",
    "stock": "integer",
    "photo": "string"
  }
}
```

### GET Products

Endpoint: `/api/products/:id`

**Request (Solicitud)**:

```json
{
  "payload": {
    "id": "integer"
  }
}

**Response (Respuesta)**:

```json
{
  "id": "integer",
  "name": "string",
  "description": "string",
  "price": "integer",
  "brand": "string",
  "stock": "integer",
  "photo": "string"
}
```

### PUT Products

Endpoint: `/api/products/:id`

**Request (Solicitud)**:

```json
{
  "payload": {
    "id": "integer",
    "name": "string",
    "description": "string",
    "price": "integer",
    "brand": "string",
    "stock": "integer",
    "photo": "string"
  }
}
```

### DELETE Products

Endpoint: `/api/products/:id`

**Request (Solicitud)**:

```json
{
  "payload": {
    "id": "integer"
  }
}

**Response (Respuesta)**:

```json
{
  "token": "string"
}
```

## Contrato de Datos - Tabla Products_variants

### POST Products_variants

Endpoint: `/api/products_variants`

**Request (Solicitud)**:

```json
{
  "payload": {
    "id_product": "integer",
    "variante": "string",
    "price": "integer",
    "iva": "integer",
    "codebar": "string",
    "sku": "string",
    "photo": "string",
    "stock": "integer"
  }
}
```

### GET Products_variants

Endpoint: `/api/products_variants/id`

**Request (Solicitud)**:

```json
{
  "payload": {
    "id": "integer"
  }
}

**Response (Respuesta)**:

```json
{
  "id": "integer",
  "id_product": "integer",
  "variante": "string",
  "price": "integer",
  "iva": "integer",
  "codebar": "string",
  "sku": "string",
  "photo": "string",
  "stock": "integer"
}
```

### PUT Products_variants

Endpoint: `/api/products_variants/id`

**Request (Solicitud)**:

```json
{
  "payload": {
    "id": "integer",
    "id_product": "integer",
    "variante": "string",
    "price": "integer",
    "iva": "integer",
    "codebar": "string",
    "sku": "string",
    "photo": "string",
    "stock": "integer"
  }
}
```

### DELETE Products_variants

Endpoint: `/api/products_variants/id`

**Request (Solicitud)**:

```json
{
  "payload": {
    "id": "integer"
  }
}

**Response (Respuesta)**:

```json
{
  "token": "string"
}
```

## Contrato de Datos - Tabla tickets

### POST Crear ticket

Endpoint: `/api/tickets`

**Request (Solicitud)**:

```json
{
  "payload": {
    "id_user": "integer",
    "id_shipping": "integer",
    "date": "integer",
    "doc_sii": "string",
    "total": "integer",
    "subtotal": "integer",
    "contact": "string",
    "telephone": "string",
    "rut": "string",
    "city": "string",
    "region": "string",
    "razon_social": "string",
    "pay_method": "string",
    "card_number": "integer",
    "address_ship": "string",
    "region_ship": "string",
    "city_ship": "string"
  }
}
```

### GET ticket

Endpoint: `/api/tickets/id`

**Request (Solicitud)**:

```json
{
  "payload": {
    "id": "integer"
  }
}

**Response (Respuesta)**:

```json
{
  "id": "integer",
  "id_user": "integer",
  "id_shipping": "integer",
  "date": "integer",
  "doc_sii": "string",
  "total": "integer",
  "subtotal": "integer",
  "contact": "string",
  "telephone": "string",
  "rut": "string",
  "city": "string",
  "region": "string",
  "razon_social": "string",
  "pay_method": "string",
  "card_number": "integer",
  "address_ship": "string",
  "region_ship": "string",
  "city_ship": "string",
  "status": "string"
}
```

## Contrato de Datos - Tabla ticket_details

### POST ticket_details

Endpoint: `/api/ticket_details`

**Request (Solicitud)**:

```json
{
  "payload": {
    "id_ticket": "integer",
    "id_product_variant": "integer",
    "quantity": "integer",
    "price": "integer",
    "iva": "integer",
    "total": "integer"
  }
}
```

### PUT ticket status

Endpoint: `/api/ticket_status/:id`

**Request (Solicitud)**:

```json
{
  "payload": {
    "id": "integer",
    "status": "string"
  }
}
```

## Contrato de Datos - Tabla shipping_cost

### GET shipping_cost

Endpoint: `/api/shipping_cost/:id`

**Request (Solicitud)**:

```json
{
  "payload": {
    "region": "string"
  }
}

**Response (Respuesta)**:

```json
{
  "id": "integer",
  "region": "string",
  "cost": "integer"
}
```

## Contrato de Datos - Tabla questions

### POST questions

Endpoint: `/api/questions`

**Request (Solicitud)**:

```json
{
  "payload": {
    "id_user": "integer",
    "id_product_variant": "integer",
    "question": "string",
    "response": "string",
    "date": "integer"
  }
}
```

## Contrato de Datos - Tabla Questions

### POST questions

Endpoint: `/api/questions`

**Request (Solicitud)**:

```json
{
  "payload": {
    "id_user": "integer",
    "id_product_variant": "integer",
    "question": "string",
    "response": "string",
    "date": "integer"
  }
}
```

### GET questions

Endpoint: `/api/questions/id`

**Request (Solicitud)**:

```json
{
  "payload": {
    "id": "integer"
  }
}

**Response (Respuesta)**:

```json
{
  "id": "integer",
  "id_user": "integer",
  "id_product_variant": "integer",
  "question": "string",
  "response": "string",
  "date": "integer"
}
```

### PUT questions (solo response)

Endpoint: `/api/questions/:id`

**Request (Solicitud)**:

```json
{
  "payload": {
    "id": "integer",
    "response": "string"
  }
}
```

### DELETE questions

Endpoint: `/api/questions/:id`

**Request (Solicitud)**:

```json
{
  "payload": {
    "id": "integer"
  }
}

**Response (Respuesta)**:

```json
{
  "token": "string"
}
```

