# Calculator App (Node.js)

A simple calculator application built with Node.js. This app provides basic arithmetic operations via a RESTful API.

## Features

- Addition, subtraction, multiplication, division
- Simple API endpoints
- Easy to extend

## Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (v18+ recommended)
- [npm](https://www.npmjs.com/)

### Installation

```bash
git clone https://github.com/jemelecek/calc-app.git
cd calculator-app
npm install
```

### Running the App

```bash
npm start
```

The server will start on `http://localhost:3000`.

## API Endpoints

| Method | Endpoint         | Description                | Example Payload           |
|--------|------------------|----------------------------|--------------------------|
| POST   | `/add`           | Add two numbers            | `{ "a": 5, "b": 3 }`     |
| POST   | `/subtract`      | Subtract two numbers       | `{ "a": 5, "b": 3 }`     |
| POST   | `/multiply`      | Multiply two numbers       | `{ "a": 5, "b": 3 }`     |
| POST   | `/divide`        | Divide two numbers         | `{ "a": 6, "b": 3 }`     |

### Example Request

```bash
curl -X POST http://localhost:3000/add \
    -H "Content-Type: application/json" \
    -d '{"a": 5, "b": 3}'
```

### Example Response

```json
{
    "result": 8
}
```

## License

MIT