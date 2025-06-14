# GoForge 🚀

GoForge is a powerful CLI tool that helps you **scaffold modern Go backend projects** in seconds.  
It is inspired by [Spring Boot](https://spring.io/projects/spring-boot) and brings convention-over-configuration to the Go ecosystem.

---

## ✨ Features

- 🔧 Quickly scaffold a complete backend project with a single command
- 🕸️ Uses [Gin](https://github.com/gin-gonic/gin) for routing
- 🗃️ Integrated with [Sqlc](https://sqlc.dev/) for type-safe SQL and database access
- 💉 Dependency injection powered by [Google Wire](https://github.com/google/wire)
- 🧱 Follows **Repository pattern** and clean modular architecture
- 📁 Prebuilt directory structure ready for production
- 🧪 Includes unit test scaffold for image watermarking (as example)

---

## 🛠️ Installation

Clone the repo and build the CLI:

```bash
git clone https://github.com/yourname/GoForge.git
cd GoForge
go build -o goforge
```

Or install globally (if you want):

go install github.com/yourname/GoForge@latest

## 🚀 Usage
Use the CLI to create a new project:

```bash
goforge new my-backend
```
This will generate:
```bash
my-backend/
├── Makefile
├── assets
├── bootstrap
├── cmd/main.go
├── config.yaml
├── go.mod
├── internal/
│   ├── config/
│   ├── db/
│   ├── handler/
│   ├── infra/
│   ├── model/
│   ├── repository/
│   ├── response/
│   ├── router/routes/
│   ├── service/
│   └── utils/
├── query/
├── schema/
└── test/
```

## 🔩 Technologies Used
- Gin — HTTP router

- Sqlc — Compile SQL to Go code

- Google Wire — Dependency Injection

- Viper — Config management

- Cobra — CLI framework

## 📚 Coming Soon
SQLite/PostgreSQL switch support

RESTful endpoint scaffolding (--resource user)

Integrated Swagger/OpenAPI generator

Docker support

## 🧑‍💻 Author
林均 Lin Kuan
Built with ❤️ from a Go developer who loves fast, clean architectures.

## 📄 License
Apache 2.0
