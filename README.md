# Task-Scheduler-with-Notification
Custom app that lets users schedule tasks and reminders, with desktop notifications and support for repeat patterns (daily, weekly, etc.).
Task Scheduler with Notifications
Task Scheduler with Notifications — Project Documentation

Project Overview:
-----------------
A desktop reminder application built using Python and Tkinter that helps users create and manage scheduled tasks. The app supports due dates, recurring tasks (daily or weekly), and sends real-time desktop notifications using the Plyer library. Task data is saved in SQLite, and unique task IDs are generated using base62 encoding.

Key Features:
-------------
- Add tasks with title, description, due date and time.
- Specify task repetition: once, daily, or weekly.
- Background thread monitors and triggers alerts on time.
- Tasks stored persistently in SQLite.
- Notification popup using cross-platform Plyer library.
- Task IDs are uniquely generated with custom base62 logic.

Technologies Used:
------------------
- Python 3.12
- Tkinter (GUI)
- SQLite3 (Local Database)
- Plyer (Desktop notifications)
- Base62 encoding (for ID logic)

File Structure:
---------------
- main.py        → App startup file.
- ui.py          → Interface layout and control events.
- db_utils.py    → Database interaction logic.
- notify.py      → Triggers plyer-based notifications.
- base62.py      → Encodes task IDs to readable short form.

How to Run:
-----------
1. Install Python 3.12 and Plyer: `pip install plyer`.
2. Open the folder in an IDE like PyCharm.
3. Run `main.py`.
4. Fill out task details and let the app notify you on schedule.

Future Enhancements:
--------------------
- Feature to edit/delete tasks.
- Display upcoming/past task list.
- Export/import task list to/from CSV or JSON.
- Add audible reminders and alarms.

