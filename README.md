# Interactive Quiz Game Website 🎮

A fully functional, interactive quiz game platform with real-time gameplay, dynamic leaderboards, and comprehensive analytics. Built with HTML, CSS, JavaScript, Node.js, Express, and MongoDB.

## 🌟 Features

- **Multi-Topic Quiz Questions**: Diverse questions covering science, history, geography, technology, sports, and more
- **Adjustable Difficulty Levels**: Easy, Medium, and Hard questions for all age groups
- **Real-Time Interactive Gameplay**: Instant feedback on answers with visual feedback
- **Dynamic Leaderboard**: Real-time ranking of players based on scores
- **Analytics Dashboard**: Comprehensive insights into player performance, popular topics, and question difficulty
- **User Profiles**: Track personal progress and statistics
- **Responsive Design**: Fully functional on desktop, tablet, and mobile devices
- **Modern UI/UX**: Clean, engaging interface that encourages participation
- **Data Persistence**: All user data, scores, and analytics stored in MongoDB

## 🛠️ Tech Stack

- **Frontend**: HTML5, CSS3, JavaScript (ES6+)
- **Backend**: Node.js, Express.js
- **Database**: MongoDB
- **Additional**: Chart.js for analytics visualization, Socket.io for real-time updates

## 📁 Project Structure

```
quiz-game-website/
├── public/
│   ├── index.html
│   ├── quiz.html
│   ├── leaderboard.html
│   ├── dashboard.html
│   ├── profile.html
│   ├── css/
│   │   ├── style.css
│   │   ├── quiz.css
│   │   ├── leaderboard.css
│   │   └── dashboard.css
│   └── js/
│       ├── main.js
│       ├── quiz.js
│       ├── leaderboard.js
│       ├── dashboard.js
│       └── api.js
├── server/
│   ├── server.js
│   ├── models/
│   │   ├── User.js
│   │   ├── Question.js
│   │   └── Score.js
│   ├── routes/
│   │   ├── auth.js
│   │   ├── quiz.js
│   │   ├── scores.js
│   │   └── analytics.js
│   ├── middleware/
│   │   └── auth.js
│   └── config/
│       └── database.js
├── data/
│   └── questions.json
├── package.json
└── .env.example
```

## 🚀 Getting Started

### Prerequisites
- Node.js (v14 or higher)
- MongoDB (local or Atlas)
- npm or yarn

### Installation

1. **Clone the repository**
```bash
git clone https://github.com/shashanksi421-afk/quiz-game-website.git
cd quiz-game-website
```

2. **Install dependencies**
```bash
npm install
```

3. **Set up environment variables**
```bash
cp .env.example .env
# Edit .env with your MongoDB connection string and settings
```

4. **Start the server**
```bash
npm start
```

5. **Open in browser**
```
http://localhost:3000
```

## 📖 Usage

### Home Page
- Welcome screen with game instructions
- Quick start button
- Links to leaderboard and dashboard

### Quiz Game
- Select difficulty level (Easy, Medium, Hard)
- Choose quiz topic or random
- Answer questions and get instant feedback
- Track score in real-time
- Submit quiz to save results

### Leaderboard
- View top 100 players globally
- Filter by time period (All Time, This Month, This Week)
- View your rank and personal best
- Compare scores with friends

### Analytics Dashboard
- Personal performance metrics
- Topic popularity analysis
- Question difficulty statistics
- Progress charts and trends
- Win rate and accuracy rates

### User Profile
- View personal statistics
- Track quiz history
- Achievement badges
- Progress over time

## 🎯 API Endpoints

### Authentication
- `POST /api/auth/register` - Register new user
- `POST /api/auth/login` - Login user
- `POST /api/auth/logout` - Logout user

### Quiz
- `GET /api/quiz/questions` - Get random questions
- `GET /api/quiz/questions/topic/:topic` - Get questions by topic
- `POST /api/quiz/submit` - Submit quiz answers

### Scores
- `GET /api/scores/leaderboard` - Get global leaderboard
- `GET /api/scores/user/:userId` - Get user scores
- `POST /api/scores/save` - Save quiz score

### Analytics
- `GET /api/analytics/dashboard` - Get dashboard data
- `GET /api/analytics/topics` - Get topic popularity
- `GET /api/analytics/difficulty` - Get difficulty analysis

## 📊 Database Schema

### User
- userId, username, email, password, createdAt, updatedAt

### Question
- questionId, text, category, difficulty, options, correctAnswer

### Score
- scoreId, userId, quizId, score, accuracy, timeSpent, answers, createdAt

## 🎨 Design Highlights

- Modern gradient backgrounds
- Smooth animations and transitions
- Intuitive navigation
- Color-coded difficulty levels
- Responsive grid layouts
- Mobile-first approach

## 🔒 Security

- Password hashing with bcrypt
- JWT authentication
- Input validation and sanitization
- CORS protection
- Rate limiting

## 📱 Responsive Breakpoints

- Desktop: 1200px and above
- Tablet: 768px to 1199px
- Mobile: Below 768px

## 📝 License

MIT License - feel free to use this project for personal or commercial purposes.

## 🤝 Contributing

Contributions are welcome! Please feel free to submit pull requests or open issues for any improvements.

## 📧 Contact

For questions or support, please reach out to shashanksi421@example.com

---

**Happy Quizzing! 🎓**