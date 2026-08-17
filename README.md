# Home Appliance Service Platform

A production-ready online platform where customers can request, book, and track AC and refrigerator servicing and repair.

## Features

### Customer
- Mobile OTP authentication
- Browse services and service categories
- Create service bookings
- Select preferred date/time and service location
- Upload attachments
- Make payments via bKash
- Track booking status
- Review completed services

### Technician
- View assigned jobs
- Accept/reject assignments
- View customer information and booking details
- Update job status
- Upload service photos
- Record used parts and charges

### Admin
- Manage services and categories
- Manage technicians
- Assign technicians to bookings
- View reports and analytics
- Manage payments and refunds
- System configuration

## Project Structure

```
service-platform/
├── backend/              # Laravel REST API
├── frontend/             # Vue 3 + TailAdmin application
├── docker/               # Docker configuration
├── docs/                 # Documentation
├── .github/workflows/    # CI/CD pipelines
├── docker-compose.yml
├── AGENTS.md
├── CONTRIBUTING.md
└── .gitignore
```

## Technology Stack

### Backend
- Laravel 11
- PHP 8.3+
- MySQL 8.0+
- Redis
- Laravel Sanctum
- REST API

### Frontend
- Vue 3
- Vite
- Vue Router
- Pinia
- Tailwind CSS
- TailAdmin Vue

## Getting Started

See [CONTRIBUTING.md](./CONTRIBUTING.md) for development setup instructions.

## Documentation

Detailed documentation is available in the `/docs` directory.

## License

Proprietary - Home Appliance Service Platform
