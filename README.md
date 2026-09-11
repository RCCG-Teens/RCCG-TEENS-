CITY OF PRAISE TEENS - SUPABASE VERSION

This version replaces the local SQLite database with Supabase. Accounts, Teen IDs, sessions, shared check-ins and history are stored online.

1. Create a Supabase project at https://supabase.com/
2. In Supabase, open SQL Editor and run supabase-schema.sql.
3. Go to Project Settings > API and copy the Project URL and service_role key. NEVER put the service_role key in public/index.html.
4. Copy .env.example to .env.
5. Put your Supabase values in .env.
6. Optional: add an OpenAI API key for Daniel GPT.
7. Open Terminal in this folder and run: npm.cmd install
8. Run: npm.cmd start
9. Open: http://localhost:3000

Registration creates a Teen ID such as COP-2026-000001. The teen logs in later using that Teen ID and the password they created.

The database is shared because records are stored in Supabase, not browser localStorage. Personal reflections are kept in the user's history and are not shown in the public/shared activity feed.

For production, deploy the Node server on a host with HTTPS and persistent environment variables. Keep the Supabase service-role key server-side only.
