# Setup Guide — Suman TV Production Hub

## Step 1: GitHub Pages (Hosting)

1. Go to github.com → Sign in (or create free account)
2. Click **+ New repository**
3. Name it: `sumantv-hub`
4. Set to **Public**
5. Click **Create repository**
6. Upload these 4 files: `index.html`, `README.md`, `404.html`, `.nojekyll`
7. Go to **Settings → Pages → Source → Deploy from branch → main → / (root)**
8. Click **Save**
9. Your URL will be: `https://YOUR-USERNAME.github.io/sumantv-hub`

## Step 2: Allow GitHub Pages in Supabase CORS

1. Go to supabase.com/dashboard/project/njxwfgcayotvjmozhlab
2. Click **Settings → API**
3. Under **Allowed Origins / CORS** add:
   `https://YOUR-USERNAME.github.io`
4. Save

## Step 3: Add Team Members as Auth Users

For each team member:
1. Go to Supabase → **Authentication → Users → Add user**
2. Email: use the email already in team_members table (e.g. anchor1@sumantv.in)
3. Set a password and share with team member
4. They open: https://YOUR-USERNAME.github.io/sumantv-hub and log in

## Step 4: Update Real Names & Emails

In Supabase → Table Editor → team_members:
- Update `full_name` to real names (e.g. "Anchor 1" → "Ravi Kumar")  
- Update `email` to real emails
- These will show in the dashboard automatically

## Adding More Doctors

In Supabase → Table Editor → doctors:
- Click **Insert row**
- Fill: doctor_id (STV-DR-013), full_name, specialty, hospital, city
- Or use SQL Editor to bulk insert

## Updating a Project Stage

In Supabase → Table Editor → projects:
- Find the project row
- Click the `stage` column
- Select new stage from dropdown
- Changes reflect immediately for all users
