# Docker Compose Confluence

A Docker Compose configuration to run [Confluence](https://www.atlassian.com/software/confluence) behind a [Traefik](https://traefik.io/) reverse proxy.

## Usage

1. Clone this repository.
2. Copy `.env.example` to `.env` and modify the variables.
3. Run `docker-compose up -d`.

## Installation

When setting up for the first time, you'll need to configure Confluence. When asked what kind of environment you're setting up, specify it's a production environment. When asked to set up the database, specify you're using your own database and fill in the following details:
- Database type: `PostgreSQL`
- Hostname: `postgres`
- Port: `5432`
- Database: `confluence`
- Username: `confluence`
- Password: the password you set in `.env`
