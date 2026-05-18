# Supabase Keep-Alive Monitor

This repository contains a GitHub Actions cron job that prevents my 5 Supabase free-tier projects from being paused due to 7 days of inactivity.

### How it works
- Runs **3 times per week** on chosen days
- Connects directly to each Supabase PostgreSQL database
- Executes a simple `SELECT 1` query (this counts as real activity)
- No need to create ping endpoints in Django projects

### Schedule
Runs every **Tuesday, Thursday, Saturday at 03:30 UTC**

Last run: GitHub shows it automatically.