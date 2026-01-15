# Expense Tracker

A clean, full-stack web application for tracking personal expenses with multi-user support and PDF reporting.

## What it does

Track your daily expenses across different categories, filter by month, and generate PDF reports. Built this to learn full-stack development and understand how authentication works in Flask.

The app includes a "Lent" category for money you've lent to others. When they pay you back, you can mark it as settled without deleting the record.

## Tech Stack

**Backend:**
- Flask (Python web framework)
- SQLAlchemy (ORM)
- SQLite (database)
- Werkzeug (password hashing)

**Frontend:**
- Vanilla JavaScript
- CSS3 (no frameworks)
- Responsive design

**Other:**
- FPDF for PDF generation
- Gunicorn for deployment

## Features

- User authentication (register/login/logout)
- Add, edit, delete expenses
- 6 categories: Food, Travel, Study, Entertainment, Lent, Other
- Monthly expense filtering
- Dark/light theme toggle
- PDF report generation
- Mobile responsive
- Multi-user support with data isolation

## Local Setup

```bash
# Clone the repo
git clone https://github.com/yourusername/expense-tracker.git
cd expense-tracker

# Create virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Run the app
python app.py
```

Open http://localhost:5000

## Project Structure

```
expense-tracker/
├── app.py              # Main Flask application
├── models.py           # Database models
├── requirements.txt    # Python dependencies
├── static/
│   ├── style.css      # All styles (dark/light themes)
│   └── script.js      # Frontend interactions
└── templates/
    ├── login.html
    ├── register.html
    ├── index.html     # Main dashboard
    └── edit_expense.html
```

## Usage

1. Register an account
2. Add expenses with amount, category, date, and optional notes
3. View total active expenses
4. Filter expenses by month
5. Edit or delete expenses as needed
6. For money lent to friends, use "Lent" category and click "Settle" when paid back
7. Download PDF reports anytime

## Known Issues

- Database resets on Render free tier after ~15 min inactivity
- PDF generation only supports ASCII characters (no emojis in notes)

## Future Improvements

- [ ] Add expense categories customization
- [ ] Chart/graph visualization
- [ ] Export to CSV
- [ ] Recurring expenses
- [ ] Budget limits and alerts
- [ ] Split expenses between users

##  Live Demo

[https://expense-tracker-sxf5.onrender.com]

## Admin Access (for portfolio review)

Demo admin credentials available on request.

## License

MIT License - feel free to use this for learning or your own projects.

## Contact

Questions? Open an issue or reach out on [www.linkedin.com/in/kirtan-jogani-b55414315].

---

Built this while learning Flask and web development. Code suggestions welcome.
