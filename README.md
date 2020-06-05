# Commuter Wallet

Commuter Wallet helps you navigate your commute benefits and transport options to get to and from work.

Originally created by [Interline Technologies](https://www.interline.io) to support the [Bay Area Fair Value Commuting Demonstration](https://www.transit.dot.gov/sites/fta.dot.gov/files/FTA%20MOD%20Project%20Description%20-%20Palo%20Alto.pdf) project. Now available as open-source software and as a hosted service from Interline.

## Dependencies

- Ruby (as specified in `.ruby-version`) and Bundler (as specified in `Gemfile.lock`)
- Node (as specified in `.nvmrc`) and Yarn
- Postgres (configured by `config/database.yml` or `DATABASE_URL`)
- Redis
- SMTP (configured by `config/initializers/email.rb`)
- headless Chrome for integration/system tests

## Configuration

Environment Variable     | Required | Example Value
-------------------------|----------|------------------------------------
COMMUTER_WALLET_HOST     | no       | 
COMMUTER_WALLET_PROTOCOL | no       | `https`
SENDGRID_API_KEY         | no       |
RAILS_FORCE_SSL          | no       | `true`
PELIAS_API_KEY           | yes      | 
ENABLE_FRESHCHAT         | no       | `true`
