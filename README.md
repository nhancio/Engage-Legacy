
# Engage-Legacy — original web application

The preserved web predecessor to [Engage](https://github.com/nhancio/Engage). A job matching application inspired by dating app UI, connecting job seekers with employers through an intuitive swipe interface.

## Features

- 🔐 **LinkedIn OAuth Authentication** - Secure login with Supabase
- 🎤 **Voice-to-Profile** - Use voice input with Gemini AI to create structured profiles
- 💼 **Dual Mode** - Switch between job seeker and employer modes
- 📊 **Profile Management** - Save and manage profiles in Supabase database
- 🎯 **Smart Matching** - Swipe through jobs or candidates to find matches

## Tech Stack

- **Frontend**: React + TypeScript + Vite
- **UI**: Tailwind CSS + Radix UI + Motion
- **Database**: Supabase (PostgreSQL)
- **Authentication**: Supabase Auth with LinkedIn OAuth
- **AI**: Google Gemini API for voice-to-text and profile extraction

## Quick Start

1. **Install dependencies:**
   ```bash
   npm install
   ```

2. **Set up environment variables:**
   Create a `.env` file with:
   ```env
   VITE_SUPABASE_URL=your_supabase_url
   VITE_SUPABASE_ANON_KEY=your_supabase_key
   VITE_GEMINI_API_KEY=your_gemini_key
   ```

3. **Set up database:**
   - Run the SQL script from `supabase-schema.sql` in your Supabase SQL Editor
   - Configure LinkedIn OAuth in Supabase Authentication settings

4. **Run the development server:**
   ```bash
   npm run dev
   ```

For detailed setup instructions, see [SETUP.md](./SETUP.md).

## Project Structure

```
src/
├── components/       # React components
├── contexts/         # React contexts (Auth)
├── lib/              # Utilities and services
│   ├── supabase.ts   # Supabase client
│   ├── gemini.ts     # Gemini API integration
│   └── profiles.ts   # Profile management
└── data/             # Mock data and types
```

## Voice Profile Creation

1. Click the microphone button
2. Speak about yourself (job seeker) or the job (employer)
3. AI processes your voice and extracts structured data
4. Review and save your profile

## Browser Compatibility

- Voice recognition works best in Chrome or Edge
- All other features work in modern browsers

## License

This project is based on a Figma design template.
  