# Football Scouter

This repository hosts the initial code for **Football Scouter**, a web-based application for scouting high school football opponents. The project aims to simplify collection and analysis of play data for effective game planning.

## Goals

- Create opponent-specific databases with teams, games, formations and plays.
- Rapid play entry with keyboard shortcuts and auto-incremented play numbers.
- Automated analysis to generate scouting reports with run/pass tendencies, directional stats and success metrics.
- Provide a modern full-stack application ready for deployment.

## Tech Stack

- **Frontend**: Next.js 14 with React and TypeScript.
- **Backend**: Next.js API routes and server-side rendering.
- **Database**: Prisma ORM using SQLite in development and PostgreSQL in production.
- **Styling**: Tailwind CSS.
- **Deployment**: Configurable for Vercel/Netlify with Docker support.

## Data Model Overview

The database uses the following main tables:

- **Teams** – stores opponent details.
- **Games** – belongs to a team and contains basic game information.
- **Formations** – scoped to a team; describes offensive formations.
- **Plays** – linked to a game and formation; tracks down, distance, play type, direction and results.

Detailed schema definitions are located in the project specification.

## Key Features

1. **Team Management** – add, edit and remove opponent teams.
2. **Game Management** – schedule and track games for each team.
3. **Formation Management** – maintain a list of formations per opponent.
4. **Play Entry** – single page form for rapid data entry with modal formation creation.
5. **Data Visualization** – sortable, filterable play table with CSV export.
6. **Scouting Reports** – automated analytics for tendencies and success metrics.

## Development Phases

1. **Phase 1** – Database setup, team and game management, basic play entry.
2. **Phase 2** – Advanced play entry form, formation management, play table.
3. **Phase 3** – Analytics engine, scouting reports, export functions.
4. **Phase 4** – UI polish, performance tuning, deployment configuration.

## Roadmap

This repository currently contains an empty codebase. The immediate plan is to provide a minimal API route to verify the environment. Future commits will establish the database schema and begin implementing CRUD endpoints and frontend pages.

## Running the Starter Server

A simple Express server exposes one route to ensure the project runs:

```bash
npm install
node server.js
```

Visit `http://localhost:3000/api/hello` to see the "Hello World" response.

