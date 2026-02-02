# Product Inventory API

A lightweight backend API for managing products. This repository demonstrates a modular, object-oriented approach using **Node.js** and **TypeScript**, organized for clarity and maintainability.

---

## Key Features

- Full CRUD for products (create, read, update, delete)
- Search and filter products by name or category
- Pagination support for list endpoints
- Consistent input validation and structured error responses
- Configurable MongoDB connection (Atlas or self-hosted)

---

## Tech Stack

- Node.js
- Express
- TypeScript
- MongoDB (Mongoose)

---

## Project Layout

```
src/
├─ app.ts
├─ server.ts
├─ config/db.ts
├─ controllers/
├─ services/
├─ repositories/
├─ models/
└─ routes/
```

---

## Environment

Create a `.env` file at the project root with values like:

```
PORT=3000
MONGO_URI=mongodb+srv://<username>:<password>@cluster0.mongodb.net/<your_db>
```

Tip: store credentials securely and avoid committing `.env` to source control.

---

## Start the App

```bash
npm install
npm run dev
```

The server will be available at `http://localhost:3000` by default.

---

## API Endpoints

- `POST /api/products` — Create a new product
- `GET /api/products` — List products (supports search & pagination)
- `GET /api/products/:id` — Retrieve a product by ID
- `PUT /api/products/:id` — Update a product
- `DELETE /api/products/:id` — Remove a product

---

## Architecture Notes

This project follows a layered structure:

- **Controllers** — Handle HTTP layer and request/response
- **Services** — Contain business logic
- **Repositories** — Encapsulate database interactions

---

## Contributing & License

Contributions are welcome — open an issue or submit a pull request. This project is provided under the MIT License.

---

## Maintainer

Vaibhav Singh
