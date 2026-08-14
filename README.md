# Ashish Shah — Vishnu Style Website + Backend Admin

This package turns the current static website into a browser-editable CMS.

## Stack
- Frontend: HTML/CSS/JavaScript
- Backend/database/auth/storage: Supabase
- Hosting: Vercel or Netlify
- Live updates: Supabase Realtime when enabled

## Setup
1. Create a Supabase project.
2. In Supabase SQL Editor, run `supabase.sql`.
3. In Supabase Authentication > Users, create your private admin user/email + password.
4. Copy the project URL and anon/publishable key into `public/config.js`.
5. Deploy the project folder to Vercel.
6. Open `/admin.html`, sign in, and edit the content.
7. Save. The public homepage reads from Supabase. With Realtime enabled, open pages update automatically; otherwise refresh.

## Important
The Supabase anon key is intended for browser use. Security comes from Row Level Security policies. Never put a Supabase service-role key in this project.

## Photo
The supplied website's exact portrait is included as `public/profile-photo.jpg`. The admin upload is also configured for Supabase Storage.
