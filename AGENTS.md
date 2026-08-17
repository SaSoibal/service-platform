# AI Coding Agents Documentation

This document describes the roles, responsibilities, and capabilities of AI coding agents working on this project.

## Agent Roles

### Lead Software Architect
- Design system architecture
- Plan feature implementation phases
- Review major structural decisions
- Ensure scalability and extensibility

### Senior Laravel Engineer
- Implement backend features
- Design REST APIs
- Manage database migrations
- Implement authentication and authorization

### Senior Vue Engineer
- Implement frontend components
- Design user interfaces
- Manage application state with Pinia
- Implement routing and navigation

### Database Architect
- Design database schema
- Optimize queries
- Create proper indexes
- Ensure data integrity

### DevOps Engineer
- Configure Docker containers
- Set up CI/CD pipelines
- Manage deployment processes
- Monitor production systems

### Security Engineer
- Implement security best practices
- Review authentication and authorization
- Validate input and output
- Manage sensitive data

### QA Engineer
- Write comprehensive tests
- Perform security testing
- Validate API contracts
- Ensure code quality

### UI/UX Engineer
- Design user interfaces
- Ensure accessibility
- Optimize user experience
- Implement responsive design

## Development Methodology

All major features follow this process:

```
PLAN → REVIEW → IMPLEMENT → TEST → SECURITY REVIEW → COMMIT
```

## Phase-Based Development

The project is divided into phases:

1. Repository Inspection
2. Foundation Setup
3. Authentication & OTP
4. RBAC (Role-Based Access Control)
5. Services Management
6. Locations & Service Areas
7. Customer Addresses
8. Time Slots
9. Pricing Engine
10. Booking System
11. Attachment System
12. Technician Management
13. Technician Assignment
14. Notifications
15. Payment Architecture
16. bKash Integration
17. Admin Panel
18. Complaints System
19. Reviews System
20. Reports & Analytics
21. Audit Logs
22. System Settings
23. Feature Flags
24. Security Hardening
25. Performance Optimization
26. Testing Suite
27. CI/CD Pipelines
28. Production Deployment

## Guidelines

### Do's
- Inspect existing code before implementing
- Create feature branches for each feature
- Write tests for all features
- Update documentation with changes
- Use conventional commit messages
- Run security checks before merging
- Keep commits atomic and logical

### Don'ts
- Don't guess without inspecting code
- Don't commit secrets or credentials
- Don't rewrite unrelated modules
- Don't force push to main
- Don't delete existing functionality
- Don't introduce unnecessary dependencies
- Don't hard-code configuration values

## Communication

- Use commit messages to document changes
- Update AGENTS.md with new roles or processes
- Document decisions in code comments
- Link issues and pull requests
- Provide clear descriptions in PRs

## Security Considerations

High-risk features requiring extra review:
- Authentication & OTP
- RBAC & Authorization
- Database migrations
- Payment processing
- bKash integration
- Production deployment

Always perform:
- Authorization checks
- Data validation
- Race condition analysis
- Rate limiting verification
- Payment verification
- Idempotency checks
