```markdown
# Project Setup and Commands

## Initial Setup

### Python Environment & Django
```bash
# Create virtual environment
py -m venv venv

# Activate environment (Windows)
venv\Scripts\activate

# Install Django
pip install django

# Start project and apps
django-admin startproject core .
django-admin startapp blog
django-admin startapp blog_api
```

### React Setup
```bash
# Create React app in 'blogapi' directory
npx create-react-app blogapi

# Enter React directory
cd blogapi

# Install React dependencies
npm install react-router-dom
npm install @material-ui/core
```

---

## Development Commands

### Django Backend
```bash
# Run development server
py manage.py runserver

# Check migrations (dry run)
py manage.py makemigrations --dry-run --verbosity 3

# Create actual migrations
py manage.py makemigrations

# Apply migrations
py manage.py migrate

# Create admin user
py manage.py createsuperuser
```

### React Frontend (from blogapi directory)
```bash
# Start development server
npm start
```

---

## Testing & Coverage

```bash
# Install coverage
pip install coverage

# Run tests with coverage
coverage run --omit='*/venv/*' manage.py test

# Generate HTML report
coverage html
```

---

## Additional Dependencies

### Django REST Framework
```bash
pip install djangorestframework
```

### CORS Headers
```bash
pip install django-cors-headers
```

---

## Key Notes
1. Django commands run from project root
2. React commands run from `blogapi/` directory
3. Always activate virtual environment first
4. Migration workflow: 
   `makemigrations` → `migrate`
5. Coverage report generates in `htmlcov/` directory
```

This structure features:
1. Clear section headers for different phases
2. Logical grouping of related commands
3. Annotations for important notes
4. Consistent command formatting
5. Separation of backend/frontend concerns
6. Required directory context for commands
7. Migration workflow clarification
8. Environment activation reminders

The organization follows a natural progression:
1. Initial setup
2. Regular development commands
3. Testing procedures
4. Additional installations
5. Important notes
