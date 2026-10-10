# Mesaly - Restaurant Booking Platform

A modern restaurant reservation platform built with Next.js, similar to OpenTable. Allows users to discover, explore, and book tables at their favorite restaurants quickly and seamlessly.

## 📋 Prerequisites

- **Bun**: v1.0 or higher (fast package manager)
- **Node.js**: v18.0 or higher (required by Bun)
- **Git**: for cloning the repository

> If you don't have Bun installed, download it from [bun.sh](https://bun.sh)

## 🚀 Installation

### 1. Clone the Repository

```bash
git clone <repository-url>
cd mesaly
```

### 2. Install Dependencies

```bash
bun install
```

### 3. Configure Environment Variables

Create a `.env.local` file in the project root:

```bash
cp .env.example .env.local
```

Then edit `.env.local` with your variables:

```env
# Supabase
NEXT_PUBLIC_SUPABASE_URL=your_supabase_project_url
NEXT_PUBLIC_SUPABASE_ANON_KEY=your_supabase_anon_key
SUPABASE_SERVICE_ROLE_KEY=your_supabase_service_role_key

# Application
NEXT_PUBLIC_API_URL=http://localhost:3000/api
NODE_ENV=development
```

## 🛠️ Available Commands

### Development

```bash
bun dev
```

Starts the development server at [http://localhost:3000](http://localhost:3000)

### Build

```bash
bun run build
```

Compiles the application for production.

### Production

```bash
bun start
```

Starts the server in production mode.

### Lint

```bash
bun run lint
```

Runs ESLint to check code quality.

### Format

```bash
bun run format
```

Formats code using Prettier.

### Tests

```bash
bun test
```

Runs the test suite.

## 📁 Project Structure

```
mesaly/
├── app/                      # Next.js routes and components (App Router)
│   ├── api/                  # API routes
│   ├── (auth)/               # Auth routes
│   ├── restaurants/          # Restaurant routes
│   └── page.tsx              # Home page
├── components/               # Reusable components
│   ├── ui/                   # Base components (buttons, inputs, etc)
│   ├── navbar/               # Navigation bar
│   └── filters/              # Filter components
├── lib/                      # Shared utilities and functions
│   ├── api/                  # API client
│   ├── auth/                 # Authentication logic
│   └── utils.ts              # Helper functions
├── public/                   # Static files
├── styles/                   # Global styles and CSS modules
├── supabase/                 # Supabase Edge Functions
├── .env.local                # Environment variables (never commit)
├── .env.example              # Example environment variables
├── next.config.js            # Next.js configuration
├── tsconfig.json             # TypeScript configuration
└── package.json              # Project dependencies
```

## ✨ Key Features (Planned)

- 🔍 **Search & Filtering**: Find restaurants by location, cuisine, and availability
- 📅 **Booking System**: Intuitive table reservation with real-time confirmation
- 👤 **User Profiles**: Manage reservations, favorites, and booking history
- ⭐ **Reviews & Ratings**: Users can leave reviews on restaurants
- 📍 **Location-Based Search**: Discover nearby restaurants
- 💳 **Payment Processing**: Secure transaction handling
- 📧 **Notifications**: Booking confirmations and reminders
- 🎨 **Modern UI**: Responsive and user-friendly design

## 🛡️ Security

- Row-level security (RLS) with Supabase
- Secure authentication and authorization
- Environment variables in `.env.local` (never commit to git)
- CORS configuration for API routes
- Rate limiting on API endpoints

## 🚀 Deployment

### Vercel (Recommended)

```bash
bun add -g vercel
vercel
```

Follow the on-screen instructions. [See documentation](https://vercel.com/docs/frameworks/nextjs)

The project is configured to deploy automatically on Vercel with support for Edge Functions.

## 📚 Technology Stack

**Backend & Database:**
- Supabase (PostgreSQL, Edge Functions)

**Frontend:**
- Next.js (App Router)
- React

**Hosting:**
- Vercel

## 🤝 Contributing

Contributions are welcome. Please:

1. Fork the project
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is under the MIT License. See `LICENSE` for details.

## 📧 Support

To report bugs or suggestions, open an [issue](https://github.com/yourusername/mesaly/issues) on GitHub.

---

**Last updated**: 2026-10-10
