# Contributing to Home Appliance Service Platform

## Development Setup

### Prerequisites
- Docker & Docker Compose
- Git
- Node.js 18+ (for local frontend development)
- PHP 8.3+ (for local backend development)

### Quick Start with Docker

```bash
# Clone the repository
git clone https://github.com/SaSoibal/service-platform.git
cd service-platform

# Start all services
docker-compose up -d

# Backend setup
docker-compose exec app composer install
docker-compose exec app php artisan key:generate
docker-compose exec app php artisan migrate --seed

# Frontend setup
cd frontend
npm install
cd ..
```

### Running Applications

**Backend API**: http://localhost:8000
**Frontend**: http://localhost:5173
**Admin Panel**: http://localhost:5173/admin

## Development Workflow

1. Create a feature branch:
   ```bash
   git checkout -b feature/your-feature-name
   ```

2. Make your changes following the coding standards.

3. Run tests:
   ```bash
   # Backend
   docker-compose exec app php artisan test
   
   # Frontend
   cd frontend && npm run test
   ```

4. Lint and format:
   ```bash
   # Backend
   docker-compose exec app ./vendor/bin/pint
   
   # Frontend
   cd frontend && npm run lint
   ```

5. Commit with conventional commits:
   ```bash
   git commit -m "feat(module): description of changes"
   ```

6. Push and create a Pull Request.

## Code Standards

### Backend
- PSR-12 coding standard
- SOLID principles
- Thin controllers, business logic in Services/Actions
- Tests for all features

### Frontend
- Vue 3 Composition API
- Reusable components
- Pinia for state management
- ESLint configuration

## Commit Message Format

Use conventional commits:

```
feat(auth): add mobile OTP authentication
fix(booking): prevent invalid status transition
test(payment): add payment gateway tests
docs(api): update API documentation
refactor(service): extract business logic
chore(ci): update GitHub Actions workflow
```

## Pull Request Process

1. Ensure all tests pass
2. Update documentation if needed
3. Keep commits clean and logical
4. Provide a clear description of changes
5. Link related issues

## Security

- Never commit `.env` files or secrets
- Always use environment variables for sensitive data
- Follow OWASP guidelines
- Request security review for authentication/payment changes

## Questions or Issues?

Open an issue or discussion in the repository.
