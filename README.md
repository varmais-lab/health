# Suman TV — Production Hub

A production management dashboard for Suman TV's content team.  
Built with HTML + Supabase (PostgreSQL backend).

## 🌐 Live App
**[Open Dashboard →](https://YOUR-USERNAME.github.io/sumantv-hub)**

## 👥 Team Login
Each team member logs in with their assigned email and password.

| Role | Example Email |
|---|---|
| Manager | manager@sumantv.in |
| Anchor | anchor1@sumantv.in |
| DOP | dop1@sumantv.in |
| Editor | editor1@sumantv.in |
| Publisher | publisher1@sumantv.in |

## 📋 Features
- Live project tracking across 8 production stages
- Per-project discussion threads with @mentions
- Doctor directory (100 doctors)
- Team workload view
- New project wizard
- Role-based access (each team member sees their own projects)

## 🗄️ Database
Hosted on Supabase (Mumbai region).  
Tables: projects, doctors, team_members, shoot_records, edit_records, publish_records, distribution_records, project_comments

## 🔧 Tech Stack
- Frontend: Vanilla HTML/CSS/JS (single file, no build step)
- Backend: Supabase (PostgreSQL + Auth + RLS)
- Hosting: GitHub Pages (free)
