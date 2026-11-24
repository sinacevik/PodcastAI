# PodcastAI

> Portfolio mirror of the team project maintained at
> [Travel-Assistant-Project/PodcastAI](https://github.com/Travel-Assistant-Project/PodcastAI).
> The canonical repository is the source of truth for current code and setup instructions.

PodcastAI is a team-built platform for generating and listening to personalized podcasts. The full project combines a React Native mobile client, an ASP.NET Core backend, and a Python/FastAPI AI service.

## My contribution

I built part of the project's initial backend foundation:

- added JWT token generation and authentication middleware configuration
- introduced the EF Core `AppDbContext` and PostgreSQL connection setup
- created the `User` entity and initial database migration
- added login, registration, and response DTOs
- created the initial authentication controller scaffolding

**Evidence:** [backend foundation commit](https://github.com/Travel-Assistant-Project/PodcastAI/commit/c2e44b6f67ae5e7b489c91bb4cf90d5b100d7076)

The linked commit used mock users in the first controller scaffold; it did not yet implement complete production registration or password verification. The project evolved later through the team's subsequent work. This distinction keeps the portfolio claim limited to what the commit demonstrates.

## Team project architecture

| Component | Technologies |
| --- | --- |
| Mobile client | React Native, Expo, TypeScript |
| Backend API | C#, ASP.NET Core, Entity Framework Core, Hangfire |
| AI service | Python, FastAPI |
| Data | PostgreSQL |
| Integrations | text generation, translation, and text-to-speech services |
| Communication | HTTP/REST between application services |

## What the contribution demonstrates

- configuring JWT-based authentication in ASP.NET Core
- modelling users with EF Core and PostgreSQL
- creating and applying an initial relational database migration
- separating request and response contracts with DTOs
- contributing a scoped backend foundation to a multi-service team project

## Inspect or build the canonical project

```bash
git clone https://github.com/Travel-Assistant-Project/PodcastAI.git
cd PodcastAI
dotnet restore ai-podcast-platform.sln
dotnet build ai-podcast-platform.sln
```

The mobile and AI services have their own dependencies and runtime configuration. Refer to the
[canonical repository](https://github.com/Travel-Assistant-Project/PodcastAI) for current setup instructions. Use local environment variables for database credentials, signing secrets, and third-party API keys; never commit real secrets.

## Repository status

This user-owned repository is kept as a portfolio mirror. Issues and pull requests for the active team project should be opened in the [canonical repository](https://github.com/Travel-Assistant-Project/PodcastAI).
