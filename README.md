# Kanban Task Tracker

A modern Kanban board application for managing tasks with drag-and-drop functionality.

## Features

- 📋 Kanban board with three columns: To Do, In Progress, Done
- ➕ Add, edit, and delete tasks
- 🖱️ Drag and drop tasks between columns
- 🏷️ Task priority (Low, Medium, High)
- 📅 Due date tracking
- 💾 Persistent storage with Supabase (free tier)

## Tech Stack

- **Frontend:** HTML, CSS, JavaScript (Vanilla)
- **Database:** Supabase (free tier)
- **Hosting:** Cloudflare Pages (free)

## Setup

1. Create a Supabase project at https://supabase.com
2. Create a table named `tasks` with the following columns:
   - `id` (auto-generated UUID)
   - `title` (text, required)
   - `description` (text)
   - `priority` (text: 'low', 'medium', 'high')
   - `status` (text: 'todo', 'in_progress', 'done')
   - `due_date` (date)
   - `created_at` (timestamp)

3. Update `index.html` with your Supabase credentials:
   - Replace `YOUR_SUPABASE_URL` with your project URL
   - Replace `YOUR_SUPABASE_ANON_KEY` with your anonymous public key

4. Deploy to Cloudflare Pages:
   - Push code to GitHub
   - Connect your GitHub repo to Cloudflare Pages
   - Set build command and output directory to `/`

## Usage

- Click "Add Task" to create a new task
- Drag tasks between columns to change status
- Click "Edit" to modify a task
- Click "Delete" to remove a task

## License

MIT
