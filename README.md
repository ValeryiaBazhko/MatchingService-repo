# Matching Service

This repository contains the ASP.NET Core MVC application used to collect human judgments for the final thesis **LLM Embedding-Based User Matching Using Unstructured Text Descriptions**.

Participants are shown pairs of pseudonymized profile descriptions and record a binary **Match** or **No Match** judgment. The collected responses are used to evaluate the embedding-based matching pipeline.

## Main components

- **Controllers**: Handles application routes and participant interactions.
- **Models**: Defines profile descriptions, profile pairs, and evaluation records.
- **Services**: Contains the application logic for loading pairs and storing judgments.
- **Data**: Provides the Entity Framework Core database context.
- **Views**: Contains the user interface for onboarding and profile-pair evaluation.
- **Dockerfile**: Supports containerized deployment.

## Requirements

- .NET SDK
- PostgreSQL database
- A connection string and other local configuration values

## Setup

1. Clone this repository.
2. Configure the PostgreSQL connection and other local settings.
3. Restore dependencies and run the application:

```bash
dotnet restore
dotnet run --project MatchingService/MatchingService.csproj
```

## Data and privacy

The application is designed to collect pseudonymized evaluation responses. The repository must not contain participant data, profile data, database dumps, passwords, API keys, or other sensitive configuration.

## Thesis

Valeryia Bazhko. *LLM Embedding-Based User Matching Using Unstructured Text Descriptions*. Final Thesis, University of Primorska, Faculty of Mathematics, Natural Sciences and Information Technologies, 2025/2026.
