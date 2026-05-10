# AcademiTrack

> A Ruby on Rails web application that helps university students manage their academic activities, subjects, and grade tracking in one place.

---

## About

**AcademiTrack** is a student-focused academic management system built with Ruby on Rails. It allows students to register, track their enrolled subjects, record grades, and monitor their academic progress throughout their university journey.

The application features user authentication, dynamic subject management with GPA/grade calculations, paginated listings, and a search interface — all wrapped in a clean Bootstrap UI.

---

## Features

- **User Authentication** - Secure sign-up, login, and session management via Devise
- **Subject Management** - Add, edit, and remove subjects dynamically
- **Grade Tracking** - Record grades per subject and calculate academic performance
- **Search & Filter** - Search through records using Ransack
- **Pagination** - Browse paginated lists with Will Paginate
- **File Uploads** - Attach files/documents using CarrierWave
- **Responsive UI** - Built with Bootstrap for a clean, mobile-friendly experience

---

## Tech Stack

| Layer        | Technology                          |
|--------------|-------------------------------------|
| Framework    | Ruby on Rails 4.0                   |
| Language     | Ruby, JavaScript (CoffeeScript)     |
| Styling      | CSS, Bootstrap-Sass 2.3             |
| Database     | MySQL (development), PostgreSQL (production) |
| Auth         | Devise                              |
| Search       | Ransack                             |
| Pagination   | Will Paginate                       |
| File Upload  | CarrierWave                         |
| Frontend     | jQuery, jQuery TokenInput           |

---

## Getting Started

### Prerequisites

- Ruby (recommended: 2.x)
- Rails 4.0
- MySQL (for development)
- Bundler

### Installation

```bash
# Clone the repository
git clone https://github.com/karunarathnad/university.git
cd university

# Install dependencies
bundle install

# Set up the database
rake db:create
rake db:migrate

# (Optional) Seed with sample data
rake db:seed

# Start the server
rails server
```

Then open your browser and navigate to `http://localhost:3000`.

---

## Project Structure

```
app/
├── controllers/   # Application logic
├── models/        # ActiveRecord models
├── views/         # ERB templates
└── assets/        # Stylesheets, JavaScript

db/
└── schema.rb      # Database schema

config/
└── routes.rb      # URL routing
```

---

## Database

- **Development:** MySQL 2
- **Production:** PostgreSQL (Heroku-compatible via `rails_12factor`)

---

## Deployment

This app is configured for deployment to **Heroku** out of the box using the `pg` and `rails_12factor` gems in the production group.

```bash
heroku create
git push heroku master
heroku run rake db:migrate
```

---

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/your-feature`)
3. Commit your changes (`git commit -m 'Add some feature'`)
4. Push to the branch (`git push origin feature/your-feature`)
5. Open a Pull Request

---

## License

This project is open source and available under the [MIT License](LICENSE).

---

## Author

**karunarathnad** — [GitHub Profile](https://github.com/karunarathnad)
