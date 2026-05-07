# Local Development Setup

This guide will help you set up and run this project locally.

## Prerequisites

Before you begin, make sure you have the following installed:
- **Node.js** (v14 or higher) - [Download](https://nodejs.org/)
- **npm** or **yarn** - Comes with Node.js
- **Git** - [Download](https://git-scm.com/)

## Installation Steps

### 1. Clone the Repository
```bash
git clone https://github.com/TytusPlayz1/Asking-hiring-someone-for-help-on-my-web-app.git
cd Asking-hiring-someone-for-help-on-my-web-app
```

### 2. Install Dependencies
```bash
npm install
# or if using yarn
yarn install
```

### 3. Set Up Environment Variables
Copy the example environment file and update with your values:
```bash
cp .env.example .env.local
```

Then edit `.env.local` and add your configuration:
```
NODE_ENV=development
API_URL=http://localhost:3000
DATABASE_URL=your_database_url_here
SECRET_KEY=your_secret_key_here
```

### 4. Run the Development Server
```bash
npm run dev
# or if using yarn
yarn dev
```

The application should now be running at `http://localhost:3000`

## Running Tests

```bash
npm run test
```

## Building for Production

```bash
npm run build
npm start
```

## Troubleshooting

### Port Already in Use
If port 3000 is already in use, you can specify a different port:
```bash
PORT=3001 npm run dev
```

### Dependencies Issues
If you encounter dependency issues, try:
```bash
rm -rf node_modules package-lock.json
npm install
```

### Database Connection Issues
Make sure your `DATABASE_URL` in `.env.local` is correct and your database is running.

## Need Help?

- Check the [CONTRIBUTING.md](CONTRIBUTING.md) guide
- Open an issue with the [bug report template](.github/ISSUE_TEMPLATE/bug_report.md)
- Join our Discord: https://discord.gg/6PE3WpYjZc

---

Happy coding! 🚀
