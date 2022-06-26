# Roundest - Which Pokémon is most round?

Answering all of life's toughest questions

## Why?

Why not. I [streamed most of the creation of this project if you're curious](https://www.youtube.com/watch?v=PKy2lYEnhgs). Regardless of how you feel about the idea, I think the technical details of this implementation are worth learning from.

## Getting Started

Prerequisite:

- MySQL local database (or Planetscale connection using PScale CLI)
- npm

Setup

1. Clone repo
2. `npm install`
3. Create `.env` file if one does not already exist
4. Add connection URLs for both database and shadow db to .env ([example .env file here](./.env.example))
5. Initialize database - `npx prisma migrate dev`
   - This will run `prisma db seed` underneath
6. Run dev server `npm run dev`

## TODO

- [x] Use next/image to handle image caching and better rendering
- [x] Persist data fetched from PokemonAPI
- [x] Create the results page with counting/sorting
- [ ] Better loading state between votes
