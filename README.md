 QuizStop - Real-Time Quiz Platform

A modern, interactive quiz platform built with Next.js, Supabase, and AI-powered question generation. Create and host live quizzes with real-time updates, confetti celebrations, and instant scoring!

 **Live Demo**: [https://quizstop-mduvn4brm-pcharvisrees-projects.vercel.app](https://quizstop-mduvn4brm-pcharvisrees-projects.vercel.app)

##  Features

###  **Core Quiz Features**
- **AI-Powered Question Generation** - Create quizzes on any topic using Gemini AI
- **Real-Time Multiplayer** - Host live quizzes with multiple participants
- **Auto-Timer System** - 30-second timer per question with automatic progression
- **Live Leaderboard** - Real-time score tracking and rankings
- **Session Management** - Easy join codes and participant management

###  **Engagement Features**
- **Confetti Celebrations** - Visual feedback for correct answers and winners
- **Sound Effects** - Audio feedback for join events and answer submissions
- **Question Count Selection** - Choose 5, 10, 15, or 20 questions per quiz
- **Difficulty Levels** - Easy, Medium, Hard, and Expert difficulty options
- **Real-Time Updates** - No page refresh needed - everything updates live!

###  **User Experience**
- **Modern UI** - Beautiful, responsive design with dark/light themes
- **Mobile Friendly** - Works perfectly on all devices
- **Instant Feedback** - Immediate scoring and progress updates
- **Connection Status** - Visual indicators for real-time connection health

##  Quick Start

### Prerequisites
- Node.js 18+ 
- Supabase account
- Gemini API key

### Installation

1. **Clone the repository**
   ```bash
   git clone <your-repo-url>
   cd quizstop
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Set up environment variables**
   Create a `.env.local` file:
   ```env
   NEXT_PUBLIC_SUPABASE_URL=your_supabase_url
   NEXT_PUBLIC_SUPABASE_ANON_KEY=your_supabase_anon_key
   GEMINI_API_KEY=your_gemini_api_key
   ```

4. **Set up the database**
   - Go to your Supabase project
   - Navigate to SQL Editor
   - Run the SQL script from `scripts/001_create_quiz_tables.sql`

5. **Run the development server**
   ```bash
   npm run dev
   ```

6. **Open your browser**
   Navigate to [http://localhost:3000](http://localhost:3000)

##  Tech Stack

- **Frontend**: Next.js 14, React, TypeScript
- **Styling**: Tailwind CSS, shadcn/ui components
- **Database**: Supabase (PostgreSQL)
- **Real-time**: Supabase Realtime
- **AI**: Google Gemini API
- **Deployment**: Vercel
- **Audio**: Web Audio API
- **Confetti**: canvas-confetti

##  How to Use

### For Quiz Hosts

1. **Create a Quiz**
   - Enter a topic or prompt
   - Select difficulty level
   - Choose number of questions (5/10/15/20)
   - Click "Generate Quiz"

2. **Host the Session**
   - Share the session code with participants
   - Start the quiz when ready
   - Monitor live leaderboard
   - Watch confetti celebrations!

### For Participants

1. **Join a Quiz**
   - Enter the session code
   - Enter your name
   - Wait for the host to start

2. **Play the Quiz**
   - Answer questions within 30 seconds
   - Get instant feedback with confetti
   - See your score update in real-time
   - Compete on the live leaderboard!

##  Scoring System

- **Simple & Fair**: 1 point per correct answer
- **Real-Time Updates**: Scores update instantly
- **Live Rankings**: See your position change in real-time
- **Final Results**: Complete leaderboard with percentages

##  Celebrations & Feedback

- **Correct Answer**: Green confetti burst + success sound
- **Wrong Answer**: Red sound feedback
- **New Participant**: Pop sound when someone joins
- **Quiz Winner**: Big confetti celebration
- **Quiz Complete**: Special completion confetti

##  API Endpoints

- `POST /api/generate-quiz` - Generate quiz questions
- `POST /api/sessions` - Create new quiz session
- `GET /api/sessions/[sessionId]` - Get session details
- `POST /api/sessions/join` - Join a session
- `PUT /api/sessions/[sessionId]/participants/[participantId]` - Submit answer

##  Database Schema

### Tables
- `quiz_sessions` - Stores quiz sessions and questions
- `quiz_participants` - Tracks participants and scores

### Real-time Features
- Live session updates
- Real-time participant tracking
- Instant score updates
- Live leaderboard changes

##  Deployment

### Vercel (Recommended)

1. **Connect your repository to Vercel**
2. **Set environment variables in Vercel dashboard**:
   - `NEXT_PUBLIC_SUPABASE_URL`
   - `NEXT_PUBLIC_SUPABASE_ANON_KEY`
   - `GEMINI_API_KEY`
3. **Deploy automatically on push**

### Manual Deployment

```bash
npm run build
npx vercel --prod
```

##  Customization

### Themes
- Built-in dark/light theme support
- Customizable color schemes
- Responsive design for all screen sizes

### Sounds
- Web Audio API for cross-platform compatibility
- Customizable sound effects
- Volume controls (coming soon)

### Confetti
- Multiple celebration types
- Customizable colors and patterns
- Performance optimized

##  Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request

##  License

This project is licensed under the MIT License - see the LICENSE file for details.

##  Acknowledgments

- **Supabase** for the amazing real-time database
- **Google Gemini** for AI-powered question generation
- **Vercel** for seamless deployment
- **shadcn/ui** for beautiful components
- **Tailwind CSS** for utility-first styling

##  Support

If you encounter any issues or have questions:

1. Check the [Issues](https://github.com/your-repo/issues) page
2. Create a new issue with detailed information
3. Include steps to reproduce any bugs

---

**Made with ❤️ for quiz enthusiasts everywhere!** 

*Happy Quizzing!* 🎉

