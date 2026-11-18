# Modern Full-Stack Engineering

> **A zero-to-production curriculum for mastering the web platform, backend engineering, frontend systems, cloud delivery, security, reliability, and technical judgment.**

[![Level](https://img.shields.io/badge/Level-Zero%20to%20Advanced-2563eb)](#curriculum-map)
[![Approach](https://img.shields.io/badge/Approach-Project%20Driven-059669)](#capstone-projects)
[![Quality](https://img.shields.io/badge/Quality-Production%20Focused-7c3aed)](#engineering-excellence-standard)
[![Accessibility](https://img.shields.io/badge/Accessibility-WCAG%202.2%20AA-0f766e)](#30-accessibility)

> [!IMPORTANT]
> This roadmap is not a collection of fashionable tools. Every module develops a durable engineering capability and ends with a practical **mastery gate**. Build the projects, measure the results, document the trade-offs, and revisit weak foundations.

## Navigate

- [Curriculum map](#curriculum-map)
- [Foundation and web platform](#foundation--web-platform)
- [Backend and data](#backend--data)
- [Frontend and application architecture](#frontend--application-architecture)
- [Security and real-time systems](#security--real-time-systems)
- [Delivery, cloud, and architecture](#delivery--cloud--architecture)
- [Product quality](#product-quality)
- [Career readiness](#career-readiness)
- [Capstone projects](#capstone-projects)
- [Engineering excellence standard](#engineering-excellence-standard)

## Curriculum Map

```text
HTML & CSS → CSS Frameworks → JavaScript → Async JavaScript → Browser APIs
→ Node.js & Browser Runtimes → HTTP & REST → Git & GitHub → Package Managers
→ Build Tools → Backend → Databases → ORM → React → State Management
→ Next.js → TypeScript → Authentication → Security → WebSockets → WebRTC
→ Redis → Queues & Pub/Sub → Bun → Turborepo → Testing → DevOps
→ Deployment → System Design → Accessibility → Automation → SEO
→ Interview Preparation → Projects
```

> [!NOTE]
> This sequence follows the structure in the supplied sample. TypeScript appears after Next.js in the sample, but use basic TypeScript gradually in Node.js and React projects. Module 17 then teaches TypeScript deeply and systematically.

## Execution Method

Use the same engineering loop in every module:

1. **Understand:** Learn the concepts from official documentation and small experiments.
2. **Implement:** Build the required feature without copying a complete tutorial.
3. **Verify:** Add tests, accessibility checks, security checks, and measurable acceptance criteria.
4. **Operate:** Run the software locally, inspect logs, reproduce failures, and fix defects.
5. **Document:** Record setup instructions, architecture, assumptions, and important trade-offs.
6. **Demonstrate:** Explain the design and complete the mastery gate without reading prepared notes.

> [!TIP]
> Maintain one engineering journal containing debugging notes, architecture decisions, performance measurements, accessibility findings, incident reports, and lessons from code reviews.

---

## Foundation · Web Platform

## 01. HTML and CSS

### Learn

- Semantic HTML: headings, landmarks, forms, tables, images, and metadata
- Native form validation, labels, keyboard navigation, and focus order
- CSS cascade, specificity, inheritance, box model, and positioning
- Flexbox, Grid, responsive layouts, media queries, and container queries
- Typography, spacing, colors, custom properties, transitions, and reduced motion
- Mobile-first design and browser developer tools

### Tools

HTML5, modern CSS, Chrome or Edge DevTools, Lighthouse, axe DevTools, and Figma inspection.

### Build

**Responsive Developer Portfolio**

- Home, projects, experience, and contact pages
- Responsive navigation and project grid
- Accessible contact form
- Dark and light themes using CSS custom properties
- Lighthouse checks for accessibility, performance, and SEO

### Mastery gate

Build a responsive page from a Figma design without Bootstrap or Tailwind. The page must work with keyboard navigation and remain readable on mobile, tablet, and desktop screens.

---

## 02. CSS Frameworks

### Learn

- Utility-first CSS and component-library approaches
- Responsive utility variants
- Design tokens and theme configuration
- Reusable component variants
- Avoiding unreadable utility-class duplication
- When plain CSS or CSS Modules are the better choice

### Tools

Tailwind CSS, shadcn/ui, Radix UI, and CSS Modules. Learn Bootstrap only well enough to maintain an existing project.

### Build

**Responsive Admin Dashboard**

- Sidebar, header, cards, tables, forms, dialogs, and notifications
- Dark mode
- Responsive navigation
- Reusable button, input, badge, card, and dialog variants

### Mastery gate

Create a consistent interface without scattering arbitrary colors, spacing, and sizes throughout the project.

---

## 03. JavaScript

### Learn

- Values, variables, types, operators, conditions, and loops
- Functions, scope, closures, and modules
- Arrays, objects, maps, sets, and collection methods
- Mutation, immutability, and side effects
- Prototypes, classes, composition, and `this`
- Error handling and input validation
- Memory references and garbage-collection basics
- Time and space complexity fundamentals

### Tools

JavaScript, Node.js, ESLint, Prettier, and VS Code debugger.

### Build

**Expense Tracker CLI**

- Add, update, delete, search, and categorize expenses
- Store data in JSON
- Validate user input
- Handle missing and corrupted files

**Log Analyzer**

- Parse web-server logs
- Count status codes and errors
- Identify slow and frequently requested endpoints

### Mastery gate

Solve small programming problems without tutorials, organize code into modules, debug with breakpoints, and explain common array and object operations.

---

## 04. Asynchronous JavaScript

### Learn

- Call stack, execution contexts, task queue, and microtask queue
- Callbacks, promises, and `async`/`await`
- Promise chaining and error propagation
- Sequential versus concurrent execution
- Timeouts, retries, cancellation, and exponential backoff
- Debouncing and throttling
- Race conditions in asynchronous code

### Tools

Promises, Fetch API, AbortController, Node.js timers, and browser DevTools.

### Build

**Concurrent API Aggregator**

- Fetch data from multiple APIs
- Add timeouts, cancellation, retries, and partial-failure handling
- Compare sequential and concurrent request times

Implement simplified versions of `Promise.all`, `Promise.allSettled`, a retry utility, and a concurrency limiter.

### Mastery gate

Explain the event loop clearly and debug unhandled rejections, stale requests, races, and incorrectly awaited operations.

---

## 05. Browser APIs

### Learn

- DOM creation, selection, traversal, and updates
- Event propagation, delegation, and default actions
- Forms and browser validation
- Fetch, navigation, history, and URL APIs
- Local Storage, Session Storage, cookies, and IndexedDB basics
- Intersection Observer and Resize Observer
- Clipboard, notifications, and file APIs
- Browser rendering and performance basics

### Build

**Vanilla JavaScript Kanban Board**

- Create, edit, move, filter, and delete tasks
- Drag-and-drop and keyboard alternatives
- Local persistence
- Import and export
- Undo support

### Mastery gate

Build an interactive browser application without React and explain event propagation, storage choices, request cancellation, and rendering bottlenecks.

---

## 06. Node.js and Browser Runtimes

### Learn

- JavaScript engines and host environments
- Node.js runtime, event loop, libuv, and non-blocking I/O
- CommonJS and ES Modules
- Buffers and streams
- Filesystem, process, path, events, and crypto modules
- Environment variables and process signals
- Browser sandbox versus server permissions
- Worker threads and child processes at a practical level

### Tools

Node.js LTS, `node`, `npm` or `pnpm`, `tsx`, and Node.js Inspector.

### Build

**File Processing Pipeline**

- Stream a large CSV file
- Validate and transform rows
- Write valid and invalid results separately
- Report progress and processing time
- Stop gracefully on a termination signal

### Mastery gate

Explain why Node.js handles I/O-heavy workloads well, when CPU-heavy work becomes a problem, and how streams avoid loading entire files into memory.

---

## 07. HTTP and REST

### Learn

- DNS, IP, ports, TCP, TLS, HTTP, and HTTPS
- Request methods, headers, bodies, status codes, and content types
- Cookies, caching, compression, CORS, and content negotiation
- REST resources and consistent error models
- Filtering, sorting, pagination, and versioning
- Idempotency
- Webhooks and signature verification
- OpenAPI contracts

### Tools

`curl`, Bruno or Postman, HTTPie, OpenAPI, Swagger UI, and browser Network tools.

### Build

**HTTP Server Using Node.js Core APIs**

- Routing and JSON parsing
- Headers and status codes
- Request IDs and logs
- Validation and central error handling
- Graceful shutdown

Write an OpenAPI contract for the server before introducing Express or NestJS.

### Mastery gate

Inspect a raw HTTP request, diagnose CORS and caching problems, choose appropriate status codes, and design predictable REST endpoints.

---

## 08. Git and GitHub

### Learn

- Working tree, staging area, commits, branches, and remotes
- Merge, rebase, conflict resolution, and cherry-pick
- Restore, reset, revert, and reflog
- Pull requests and code review
- Tags, releases, and semantic versioning
- Trunk-based development and short-lived branches
- GitHub Issues, Projects, Actions, Releases, and Dependabot

### Tools

Git CLI, GitHub, GitHub CLI, Husky, and lint-staged.

### Build

Manage every roadmap project through issues and pull requests. Add a README, contribution guide, pull-request template, issue templates, release tags, and branch protection to the main capstone repository.

### Mastery gate

Recover from common Git mistakes, resolve conflicts safely, review a pull request, and explain merge versus rebase trade-offs.

---

## 09. Package Managers

### Learn

- `package.json`, scripts, dependencies, and development dependencies
- Lockfiles and deterministic installations
- Semantic version ranges
- Peer and optional dependencies
- Package publishing and versioning
- npm registry security
- Workspaces
- Dependency auditing and supply-chain risk

### Tools

Prefer pnpm for projects and monorepos. Understand npm and Yarn because existing repositories use all three.

### Build

**Reusable Utility Package**

- TypeScript source
- ESM and CommonJS outputs if required
- Type declarations
- Tests and documentation
- Semantic versioning
- Local publishing with a test registry or package tarball

### Mastery gate

Explain the lockfile, diagnose dependency conflicts, avoid unsafe lifecycle scripts, and publish a correctly versioned package.

---

## 10. Build Tools

### Learn

- Parsing, transpilation, bundling, minification, and source maps
- Development servers and Hot Module Replacement
- Tree shaking and code splitting
- Environment-variable replacement
- Asset handling
- Browser compatibility targets
- Development versus production builds

### Tools

Vite, esbuild, SWC, Rollup, and webpack concepts. Use Vite for most applications.

### Build

Create a small application with:

- Development and production modes
- Lazy-loaded routes
- Environment-specific configuration
- Bundle analysis
- Source maps
- Optimized images and assets

### Mastery gate

Explain what the build tool does, diagnose a production-only build error, and identify an unnecessarily large dependency in a bundle report.

---

## Backend · Data

## 11. Backend Development

### Learn

- Routing, middleware, validation, and central error handling
- Controllers, services, repositories, and domain modules
- Configuration and secret management
- Structured logging and request correlation
- File uploads and background jobs
- Rate limiting and abuse controls
- Health, readiness, and graceful shutdown
- Modular monolith architecture
- Serverless backend fundamentals

### Tools

Node.js, TypeScript, Fastify or Express, NestJS for structured applications, Zod or TypeBox, Pino, and OpenAPI.

### Build

**Production Task Management API**

- Users, teams, projects, tasks, comments, and audit records
- Filtering, sorting, and cursor pagination
- Consistent validation and error responses
- Structured logs
- Health endpoints
- OpenAPI documentation

### Enterprise extension

Rebuild one bounded module using Java, Spring Boot, Spring Security, Spring Data JPA, Flyway, JUnit 5, and Testcontainers.

### Mastery gate

Build a documented API with clean boundaries, validation, error handling, logs, tests, and reliable startup and shutdown behavior.

---

## 12. Databases

### Learn

#### PostgreSQL and SQL

- Relational modeling, keys, constraints, and normalization
- Joins, aggregation, subqueries, CTEs, and window functions
- Transactions, isolation levels, locks, and deadlocks
- Indexes, query plans, and `EXPLAIN ANALYZE`
- Cursor pagination, connection pooling, backups, and migrations

#### MongoDB

- Documents, embedding versus referencing, indexes, and aggregations
- Atomic updates and consistency trade-offs
- When the document model is appropriate

#### Redis introduction

- Key-value storage, expiration, cache-aside, sessions, and rate limiting

### Tools

PostgreSQL, `psql`, DBeaver, MongoDB Compass, Redis CLI, and Testcontainers.

### Build

**Project Management Data Layer**

- PostgreSQL schema with constraints and indexes
- Reporting queries
- Transaction-safe task assignment
- Query-plan analysis

**Database Decision Exercise**

Implement a product catalog in PostgreSQL and MongoDB, then record the access-pattern and consistency trade-offs in an Architecture Decision Record.

### Mastery gate

Choose databases from requirements rather than fashion, write meaningful SQL, use transactions correctly, and optimize only after measuring query plans.

---

## 13. ORM

### Learn

- Object-relational mapping and the impedance mismatch
- Schema-first versus code-first workflows
- Migrations and deployment safety
- Relations, transactions, and connection pooling
- Lazy and eager loading
- N+1 queries
- Raw SQL escape hatches
- Optimistic concurrency

### Tools

Drizzle or Prisma for Node.js. JPA/Hibernate for Spring Boot. Flyway or Liquibase for enterprise migrations.

### Build

Add an ORM to the task API:

- Repositories and transactions
- Repeatable schema migrations
- Seed data
- Query logging
- Integration tests against PostgreSQL
- One performance-sensitive query written in raw SQL

### Mastery gate

Inspect generated queries, detect N+1 behavior, write safe migrations, and know when not to force a complex query through an ORM.

---

## Frontend · Application Architecture

## 14. React

### Learn

- Components, JSX, props, state, and composition
- Render behavior and reconciliation
- Controlled forms
- Hooks and custom hooks
- Effect dependencies and avoiding unnecessary effects
- State colocation and lifting state
- Error boundaries
- Client state versus server state
- Accessibility and performance profiling

### Tools

React, Vite, React Router, TanStack Query, React Hook Form, Zod, React Testing Library, and Storybook.

### Build

**Issue-Tracking Frontend**

- Authentication screens
- Issue list, details, search, filters, and cursor pagination
- Accessible create and edit forms
- Optimistic updates
- Loading, empty, error, and offline states
- Integration with the existing backend API

### Mastery gate

Choose appropriate component boundaries, avoid unnecessary global state and effects, and diagnose extra renders using React DevTools.

---

## 15. State Management

### Learn

- Local, lifted, contextual, URL, form, and server state
- Reducers and state machines
- Immutable updates
- State normalization
- Cache invalidation
- Optimistic updates
- Persistence and synchronization
- Avoiding global-state overuse

### Tools

React Context and `useReducer`, TanStack Query, Zustand for small shared client state, Redux Toolkit for complex application workflows, and XState when explicit state machines help.

### Build

Extend the issue tracker with:

- URL-driven filters
- TanStack Query caching and invalidation
- Optimistic mutations with rollback
- Small persistent preference store
- Explicit workflow state for a multi-step form

### Mastery gate

Explain why each piece of state lives where it does and distinguish remote server state from local interface state.

---

## 16. Next.js

### Learn

- App Router and nested layouts
- Server and Client Components
- Static, dynamic, and streamed rendering
- Route Handlers and Server Actions
- Loading, error, and not-found boundaries
- Caching and revalidation
- Image and font optimization
- Metadata and SEO
- Middleware and edge-runtime trade-offs

### Tools

Next.js, React, Tailwind CSS, Vercel for quick previews, and AWS or Azure for deeper deployment learning.

### Build

**Content and Commerce Application**

- Public catalog and content pages
- Search and filtering
- Shopping cart
- Checkout simulation
- Order history
- Administrative pages
- Suitable server/client boundaries
- Metadata, sitemap, and structured data

### Mastery gate

Justify the rendering and caching strategy of each major route and prevent server-only secrets from entering browser bundles.

---

## 17. TypeScript Deep Dive

### Learn

- Structural typing
- Interfaces and type aliases
- Unions, intersections, and discriminated unions
- Generics and constraints
- Conditional, mapped, indexed-access, and template-literal types
- Utility types
- Module declarations
- Type narrowing and exhaustive checking
- `unknown`, `never`, and safe error handling
- Compile-time types versus runtime validation

### Tools

TypeScript with strict settings, `tsc`, `tsx`, Zod, and API-client generation from OpenAPI.

### Build

**Typed Full-Stack Monorepo**

- Shared API contracts
- Generated API client
- Strict TypeScript across frontend and backend
- Discriminated API result types
- Runtime validation at trust boundaries
- Reusable generic utilities without unsafe assertions

### Mastery gate

Keep `any` out of application code, model success and error states precisely, and use advanced types only when they improve correctness and readability.

---

## Security · Real-Time Systems

## 18. Authentication

### Learn

- Password hashing with Argon2id or bcrypt
- Cookie-based sessions
- Access and refresh tokens
- JWT benefits and common misuse
- OAuth 2.0 and OpenID Connect
- Email verification and password reset
- Session rotation and revocation
- Multi-factor authentication and passkey concepts
- Role, permission, and resource-level authorization

### Tools

Auth.js, Better Auth, Keycloak, Microsoft Entra ID, Amazon Cognito, Auth0, or Clerk. Use managed identity for production when it reduces risk and operational work.

### Build

**Identity and Access Module**

- Registration and sign-in
- Secure session cookies
- Email verification
- Password reset with expiring single-use tokens
- OAuth/OIDC login
- Role and resource ownership checks
- Session management and audit history

### Mastery gate

Explain session and token trade-offs, secure browser authentication correctly, and enforce authorization on every protected backend operation.

---

## 19. Security

### Learn

- OWASP Top 10
- Injection, XSS, CSRF, SSRF, path traversal, and broken access control
- Secure headers and Content Security Policy
- CORS configuration
- Validation, escaping, and output encoding
- Secrets and key rotation
- Dependency and software-supply-chain security
- Encryption in transit and at rest
- Threat modeling and secure logging
- Rate limiting, CAPTCHA trade-offs, and DDoS protection layers

### Tools

OWASP ZAP, CodeQL, Dependabot, Trivy, GitHub secret scanning, Semgrep, and cloud secret managers.

### Build

Conduct a security review of the full-stack application:

- Create a data-flow threat model
- Run SAST, dependency, secret, container, and DAST scans
- Fix verified findings
- Add security tests
- Document accepted risks and false positives

### Mastery gate

Demonstrate protections against broken access control, injection, XSS, CSRF, credential leakage, and abusive request patterns.

---

## 20. WebSockets

### Learn

- HTTP upgrade and persistent connections
- Connection lifecycle
- Rooms and channels
- Authentication and authorization
- Heartbeats, reconnects, and backoff
- Ordering, acknowledgement, and duplicate handling
- Backpressure
- Horizontal scaling using Redis adapters or brokers
- When Server-Sent Events are simpler

### Tools

WebSocket API, `ws` or Socket.IO, Redis, and k6 WebSocket tests.

### Build

**Real-Time Collaboration or Chat Application**

- Authenticated connections
- Presence and typing indicators
- Persisted messages
- Delivery acknowledgement
- Reconnection and missed-message recovery
- Per-user and per-room rate limits

### Mastery gate

Handle reconnects, slow clients, duplicate messages, expired authentication, and multiple backend instances.

---

## 21. WebRTC

### Learn

- Peer-to-peer media concepts
- Signaling
- Session Description Protocol
- ICE candidates
- STUN and TURN
- NAT traversal
- Media streams and data channels
- Mesh limitations and SFU architecture
- Permissions, privacy, and connection diagnostics

### Tools

Browser WebRTC APIs, a WebSocket signaling server, coturn, and LiveKit or mediasoup for advanced multiparty systems.

### Build

**One-to-One Video Calling Application**

- Room creation
- WebSocket signaling
- Camera and microphone controls
- Screen sharing
- Reconnect and device-selection handling
- TURN fallback

### Mastery gate

Explain why signaling is separate from media, diagnose ICE failures, and explain why multi-user video usually requires an SFU.

---

## 22. Redis Deep Dive

### Learn

- Strings, hashes, lists, sets, sorted sets, bitmaps, and streams
- Expiration and eviction policies
- Cache-aside and write-through concepts
- Cache stampede protection
- Sessions and rate limiting
- Pub/sub versus Redis Streams
- Transactions and Lua scripts
- Distributed locks and Redlock controversies
- Persistence and replication basics

### Build

Add Redis to the primary application for:

- Session storage
- Rate limiting
- Hot-data caching
- Idempotency records
- Leaderboards or priority ordering
- Cache hit-rate and latency metrics

### Mastery gate

Design cache invalidation explicitly, handle Redis downtime safely, and avoid treating Redis as the permanent source of truth unless the use case supports it.

---

## 23. Queues and Pub/Sub

### Learn

- Work queues versus pub/sub
- At-most-once, at-least-once, and effectively-once processing
- Consumer groups
- Retries and exponential backoff
- Dead-letter queues
- Idempotent consumers
- Ordering and partitioning
- Outbox and inbox patterns
- Event schema compatibility
- Backpressure and lag monitoring

### Tools

BullMQ for Redis-backed jobs, RabbitMQ for traditional messaging, Apache Kafka for durable event streams, and AWS SQS/SNS or Azure Service Bus in cloud systems.

### Build

**Notification and Order Event Pipeline**

- Transactional outbox
- Email and in-app notification workers
- Retries and dead-letter handling
- Duplicate-event protection
- Replay support
- Queue-depth and processing-latency dashboards

### Mastery gate

Prove that duplicate delivery cannot duplicate business effects and that failed events can be inspected, retried, and replayed safely.

---

## 24. Bun

### Learn

- Bun runtime, package manager, bundler, and test runner
- Node.js compatibility
- Performance claims versus measured application performance
- Migration and ecosystem risks
- Situations where Node.js remains the safer production choice

### Tools

Bun and its built-in package, build, test, and runtime commands.

### Build

Run one small API and test suite under both Bun and Node.js. Compare installation time, startup time, test speed, compatibility problems, and production readiness.

### Mastery gate

Choose Bun from measured benefits and compatibility requirements, not benchmark headlines.

---

## 25. Turborepo and Monorepos

### Learn

- Monorepo benefits and costs
- Applications versus shared packages
- Workspace dependency boundaries
- Task graphs and caching
- Affected builds
- Shared TypeScript, linting, UI, contracts, and database packages
- Versioning and release strategies
- Preventing accidental package coupling

### Tools

pnpm workspaces, Turborepo, Changesets, and optionally Nx for larger enterprise workspaces.

### Build

Structure the capstone as:

```text
apps/web
apps/api
apps/worker
packages/ui
packages/contracts
packages/database
packages/config
packages/testing
```

Configure cached builds, tests, linting, type checks, and affected-package CI.

### Mastery gate

Run only required pipeline tasks after a change and maintain clear package ownership without circular dependencies.

---

## 26. Testing

### Learn

- Unit, integration, component, API, contract, end-to-end, load, and security tests
- Test pyramid and practical testing strategy
- Mocks, stubs, fakes, and test data factories
- Behavior-focused assertions
- Deterministic tests and clock control
- Database and container-based integration testing
- Flaky-test diagnosis
- Coverage as a diagnostic, not a target by itself

### Tools

Vitest or Jest, React Testing Library, Playwright, Supertest, MSW, JUnit 5, Mockito, Testcontainers, Pact, and k6.

### Build

Test the critical flow:

- Registration and login
- Creating and updating a project
- Checkout or order placement
- Queue-driven notification
- Authorization failure
- Database rollback
- Browser end-to-end flow
- Load test for the busiest API

### Mastery gate

Select the correct test layer, reproduce failures consistently, remove flaky behavior, and prove fixes with regression tests.

---

## Delivery · Cloud · Architecture

## 27. DevOps

### Learn

- Linux files, permissions, processes, signals, services, and logs
- Bash scripting
- Docker images, containers, networks, volumes, and registries
- Multi-stage builds and non-root containers
- Docker Compose
- CI/CD principles and quality gates
- Infrastructure as Code
- Configuration and secret management
- Logs, metrics, traces, and operational runbooks

### Tools

Ubuntu, Bash, Docker, Docker Compose, GitHub Actions, Terraform, OpenTelemetry, Prometheus, Grafana, and Trivy.

### Build

- Containerize web, API, worker, PostgreSQL, and Redis services
- Run the system with Docker Compose
- Add health checks
- Scan images
- Build a pipeline for lint, type check, tests, build, scan, and image publishing
- Provision a staging environment with Terraform

### Mastery gate

Create a reproducible local and CI environment from a clean machine and diagnose container, network, configuration, and pipeline failures.

---

## 28. Deployment

### Learn

- Domains, DNS, TLS certificates, CDNs, reverse proxies, and load balancers
- Static, server-rendered, container, and serverless deployment models
- Managed PostgreSQL and Redis
- Rolling, blue-green, and canary deployment
- Database migration safety
- Environment promotion, rollback, and disaster recovery
- Cloud IAM, networking, monitoring, backups, and cost control
- Kubernetes fundamentals after Docker and cloud deployment

### Tools

Vercel for previews, AWS or Azure for production learning, Nginx, Amazon ECS/Fargate or Azure Container Apps, RDS/Azure Database for PostgreSQL, ElastiCache/Azure Cache for Redis, GitHub Actions, and Kubernetes/EKS/AKS only when justified.

### Build

**Production Deployment**

- CDN and HTTPS
- API behind a load balancer
- Managed PostgreSQL and Redis
- Private service networking where practical
- Least-privilege identities
- Automated migrations
- Smoke tests and rollback
- Backups, dashboards, alerts, and monthly cost estimate

### Mastery gate

Deploy without exposing every service publicly, roll back a bad release, restore application data in a practice exercise, and explain the major cost drivers.

---

## 29. System Design

### Learn

- Functional and non-functional requirements
- Capacity and storage estimates
- Throughput, latency, availability, durability, consistency, and cost
- API and data-model design
- Caching, replication, partitioning, and sharding
- Load balancing and autoscaling
- Queues and event-driven workflows
- Rate limiting and abuse protection
- Object storage, CDNs, and search
- Failure modes and graceful degradation
- Service boundaries and microservices trade-offs
- Observability, security, and multi-region basics

### Design exercises

- URL shortener
- Notification system
- Chat platform
- File-sharing system
- E-commerce checkout
- Video-processing pipeline
- Distributed job scheduler

### Build

Create a design packet for the capstone containing requirements, estimates, API contracts, database model, C4 diagrams, sequence diagrams, cache strategy, failure analysis, security model, SLOs, observability plan, cost estimate, and load-test evidence.

### Mastery gate

Defend a design with quantified assumptions and clearly explain why simpler alternatives were rejected.

---

## Product Quality

## 30. Accessibility

### Learn

- WCAG 2.2 principles and common success criteria
- Semantic HTML and accessible names
- Keyboard navigation and focus management
- Forms, validation, and error announcements
- Color contrast and non-color indicators
- Reduced motion
- Screen-reader testing
- Accessible dialogs, menus, tabs, tables, and live regions

### Tools

axe DevTools, Lighthouse, Accessibility Insights, NVDA on Windows, VoiceOver on Apple platforms, and Playwright accessibility checks.

> [!WARNING]
> Automated scanners find only part of the accessibility defects in a product. Validate keyboard operation, focus order and visibility, reflow at narrow viewports, accessible names, alternative text, contrast, status announcements, error recovery, and screen-reader interaction manually. Use native HTML before ARIA, and use the WAI-ARIA Authoring Practices Guide for widget interaction patterns rather than treating ARIA as a substitute for behavior.

### Build

Audit the capstone and fix:

- Keyboard traps
- Missing labels
- Incorrect heading hierarchy
- Weak contrast
- Inaccessible dialogs
- Unannounced validation errors
- Dynamic content that is invisible to assistive technology

### Mastery gate

Complete critical workflows using only a keyboard and test at least one workflow with a screen reader. Automated checks alone are not sufficient.

---

## 31. Automation

### Learn

- Shell automation
- Node.js scripts
- Git hooks
- GitHub Actions workflows
- Scheduled jobs
- Dependency and release automation
- Code generation
- Database backup and maintenance jobs
- Browser automation
- Idempotent scripts and safe failure behavior

### Tools

Bash, Node.js, GitHub Actions, Playwright, Renovate or Dependabot, Changesets, and cloud schedulers.

### Build

Automate:

- Development environment setup
- Linting and formatting before commits
- API client generation
- Database backups and verification
- Dependency update pull requests
- Release notes and package versioning
- Scheduled smoke tests
- Preview deployments

### Mastery gate

A new contributor can clone the repository, run one documented setup command, and reach a working development environment without manual hidden steps.

---

## 32. SEO

### Learn

- Crawlability and indexability
- Titles, descriptions, canonical URLs, robots directives, and sitemaps
- Semantic content and heading structure
- Structured data using Schema.org
- Open Graph and social metadata
- Core Web Vitals
- Image optimization and responsive media
- Server rendering and metadata in Next.js
- Redirects, duplicate content, and broken links
- Search Console measurement

### Tools

Google Search Console, Bing Webmaster Tools, Lighthouse, PageSpeed Insights, Schema.org validator, and Next.js metadata APIs.

### Build

Optimize the content or commerce project with:

- Unique metadata
- Canonical URLs
- Sitemap and robots file
- Product, article, or breadcrumb structured data
- Open Graph images
- Fast page loading
- Redirect and broken-link checks

### Mastery gate

Important public pages are crawlable, provide valid structured metadata, meet realistic performance targets, and avoid duplicate-content problems.

---

## Advanced Topics That Complete the Stack

The 32-module curriculum covers the main path. The following cross-cutting topics close important gaps that appear in real production systems.

### API Styles and Integration

Learn GraphQL fundamentals, gRPC, Server-Sent Events, webhook design, API gateways, backward compatibility, consumer-driven contracts, generated clients, and API deprecation. REST should remain the default until another style solves a measured problem better.

**Build:** expose one read-heavy feature through GraphQL, connect two internal services with gRPC, and implement a signed, replay-safe webhook.

### Software Architecture and Design

Learn cohesion, coupling, dependency inversion, composition, ports and adapters, clean architecture trade-offs, domain-driven design fundamentals, bounded contexts, design patterns, event-driven architecture, and Architecture Decision Records. Avoid pattern-driven overengineering.

**Build:** refactor one tightly coupled module into explicit domain, application, and infrastructure boundaries. Record why the change improves testability or maintainability.

### Web Performance

Learn Core Web Vitals, the critical rendering path, bundle budgets, code splitting, image formats, lazy loading, browser caching, CDN behavior, database latency, p95/p99 response times, profiling, and capacity limits.

**Tools:** Chrome Performance panel, React Profiler, Lighthouse, WebPageTest, bundle analyzers, PostgreSQL `EXPLAIN ANALYZE`, and k6.

**Build:** establish a baseline, optimize the slowest user journey, and publish before-and-after measurements. Do not claim an improvement without data.

### Search Systems

Learn full-text search, inverted indexes, tokenization, analyzers, ranking, typo tolerance, faceting, pagination, indexing pipelines, and eventual consistency between a system of record and a search index.

**Tools:** PostgreSQL full-text search first, then Elasticsearch or OpenSearch when scale or search behavior justifies the operational cost.

**Build:** add catalog or documentation search with relevance tests, filters, highlighting, and index-rebuild support.

### Feature Flags and Safe Delivery

Learn release flags, experiment flags, operational kill switches, percentage-based rollout, user targeting, flag ownership, stale-flag removal, and the difference between deployment and release.

**Tools:** OpenFeature, LaunchDarkly, Azure App Configuration, or a small internal implementation for learning.

**Build:** release a risky feature to a small cohort, monitor errors and latency, then roll forward or disable the feature without redeploying.

### Data Privacy and Responsible Engineering

Learn data classification, data minimization, retention, deletion, auditability, consent, encryption, secrets, personally identifiable information, secure telemetry, and privacy-aware AI usage. Understand the regulations and contractual requirements that apply to the product's users and operating regions.

**Build:** create a data inventory, retention table, deletion workflow, export workflow, and log-redaction tests for the capstone.

### Documentation and Technical Communication

Learn concise READMEs, API documentation, runbooks, ADRs, RFCs, incident updates, post-incident reviews, diagrams, code-review comments, and stakeholder summaries.

**Build:** write an RFC for a major capstone change, request review, incorporate feedback, and maintain a decision log.

### AI Engineering Extension

Learn direct model APIs, structured outputs, tool calling, embeddings, retrieval-augmented generation, evaluation datasets, prompt-injection risks, permission-aware retrieval, cost and latency controls, caching, fallback behavior, and human review.

**Build:** add an evidence-grounded assistant to the capstone. Require source references, authorization checks, unsupported-answer refusal, evaluation results, and telemetry that excludes sensitive prompts.

---

## Career Readiness

## Interview Preparation

### Data Structures and Algorithms

Learn arrays, strings, hash maps, linked lists, stacks, queues, trees, heaps, tries, graphs, sorting, binary search, two pointers, sliding windows, prefix sums, recursion, backtracking, greedy algorithms, dynamic programming, union-find, and topological sorting.

For each problem:

1. Clarify constraints.
2. Write a simple correct solution.
3. Analyze time and space complexity.
4. Optimize the bottleneck.
5. Test edge cases.
6. Explain the solution without reading the implementation.

### JavaScript and TypeScript interviews

Prepare closures, event loop, promises, prototypes, modules, browser rendering, TypeScript narrowing, generics, runtime validation, and common debugging scenarios.

### Frontend interviews

Prepare accessibility, responsive layout, React rendering, state ownership, caching, forms, performance, testing, and frontend system design.

### Backend interviews

Prepare HTTP, API design, authentication, authorization, SQL, transactions, indexes, caching, queues, idempotency, concurrency, Node.js internals, and observability.

### System design interviews

Practice clarifying requirements, making estimates, drawing architecture, discussing data models, handling failure, defining SLOs, and explaining trade-offs.

### Behavioral interviews

Prepare concise STAR examples for ownership, conflict, failure, debugging, quality improvement, difficult trade-offs, incident response, and learning an unfamiliar system.

### Interview build exercises

- Autocomplete using a trie
- Job scheduler using a priority queue
- Rate limiter using Redis
- URL shortener
- Real-time chat architecture
- Transaction-safe wallet service

---

## Capstone Projects

## Project 1: Accessible Portfolio

**Focus:** HTML, CSS, CSS frameworks, browser APIs, accessibility, and SEO.

Build a responsive portfolio with projects, articles, contact form, theme support, structured metadata, strong keyboard support, and measurable performance.

## Project 2: Task and Issue Platform

**Focus:** Node.js, HTTP, PostgreSQL, ORM, authentication, security, React, state management, and testing.

Build users, teams, projects, tasks, comments, permissions, audit history, filters, cursor pagination, notifications, and complete automated tests.

## Project 3: Production Commerce Platform

**Focus:** Next.js, TypeScript, Redis, queues, webhooks, CI/CD, deployment, accessibility, and SEO.

Build product discovery, cart, checkout simulation, inventory, orders, idempotent webhooks, administration, caching, asynchronous notifications, observability, and deployment.

## Project 4: Real-Time Collaboration Platform

**Focus:** WebSockets, Redis, pub/sub, WebRTC, presence, and failure handling.

Build rooms, chat, presence, typing indicators, screen sharing, one-to-one calls, reconnection, missed-event recovery, and horizontally scalable messaging.

## Project 5: Enterprise Order and Ledger System

**Focus:** Java, Spring Boot, PostgreSQL, Kafka, transactions, security, and Testcontainers.

Build order state transitions, inventory reservation, an immutable ledger, transactional outbox, idempotent event consumers, audit history, and concurrency tests.

## Project 6: Cloud-Native Capstone

**Focus:** Monorepos, Docker, CI/CD, AWS or Azure, Terraform, Kubernetes, observability, reliability, and system design.

Deploy the strongest previous application using secure networking, managed data services, automated rollouts, dashboards, alerts, backups, load tests, failure simulations, and a documented rollback procedure.

## Project 7: AI-Enabled Product Feature

**Focus:** AI-assisted engineering and modern product development.

Add a repository assistant, support classifier, semantic search, or documentation assistant. Require structured outputs, source grounding, a repeatable evaluation dataset, privacy controls, and human review for uncertain results.

## Optional Project 8: Web3 Introduction

**Focus:** Blockchain fundamentals without distracting from core engineering.

Build a document-proof application that stores only hashes on-chain. Learn Solidity, Foundry or Hardhat, OpenZeppelin Contracts, wallet interaction, gas costs, access control, and common smart-contract vulnerabilities.

---

## Portfolio Review Matrix

Use this matrix before presenting a project as portfolio-ready.

| Dimension | Minimum evidence |
|---|---|
| Product | Clear problem, users, workflows, and acceptance criteria |
| Code | Consistent structure, meaningful names, linting, type safety, and reviewable commits |
| UX | Responsive design, loading/empty/error states, and usable forms |
| Accessibility | WCAG 2.2 AA-oriented automated and manual checks with documented findings |
| Backend | Validation, authorization, transactions, idempotency, and predictable errors |
| Data | Constraints, migrations, indexes, query evidence, backup, and recovery plan |
| Security | Threat model, secret handling, dependency scans, and abuse protections |
| Testing | Critical-path unit, integration, end-to-end, and load evidence |
| Delivery | Reproducible build, CI/CD, staged deployment, smoke tests, and rollback |
| Operations | Logs, metrics, traces, dashboards, alerts, runbook, and incident exercise |
| Communication | README, diagrams, ADRs, release notes, and concise demo narrative |

---

## Engineering Excellence Standard

Every major project should include:

- [ ] Clear README and setup instructions
- [ ] Requirements and acceptance criteria
- [ ] Architecture and sequence diagrams
- [ ] API specification
- [ ] Database schema and repeatable migrations
- [ ] Authentication and authorization design
- [ ] Threat model and security scan results
- [ ] Unit, integration, end-to-end, and load tests
- [ ] CI/CD pipeline
- [ ] Docker-based local environment
- [ ] Deployment and rollback procedure
- [ ] Structured logs, metrics, traces, dashboards, and alerts
- [ ] Architecture Decision Records
- [ ] Operational runbook
- [ ] At least one simulated incident and root-cause analysis

## The Standard

Exceptional engineering is not measured by the number of frameworks on a résumé. It is visible in the ability to understand a problem, choose a proportionate design, ship safely, diagnose failures, protect users, and improve a system using evidence.

Build fewer projects and take them further:

**Understand → Design → Implement → Test → Secure → Deploy → Observe → Break → Recover → Improve → Explain**
