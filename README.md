# 🎵 RhythmicTunes

A modern, feature-rich music streaming web application built with React.js that delivers a complete music listening experience. Browse artists, discover new music, create playlists, and enjoy your favorite tracks with an intuitive and responsive interface.

## ✨ Features

### 🎧 Core Music Experience
- **Audio Playback**: Full-featured music player with play, pause, skip, and shuffle controls
- **Playlist Queue**: Smart queue system that plays songs in sequence from current context
- **Volume Control**: Adjustable volume slider with mute functionality
- **Progress Control**: Seek to any position in the track with visual progress bar
- **Repeat Modes**: Off, track repeat, and queue repeat with visual indicators
- **Shuffle Mode**: Random song playback with toggle functionality
- **Minimizable Player**: Collapsible audio player for better screen space management

### 📚 Music Library
- **Browse Music**: Explore featured songs, top charts, and new releases
- **Artist Discovery**: Dedicated artists page with detailed artist information and song collections
- **Search Functionality**: Search for songs, artists, and albums
- **Genre Browsing**: Explore music by different genres

### 📋 Playlist Management
- **Create Playlists**: Build custom playlists with your favorite songs
- **Playlist Controls**: Play entire playlists, delete songs, and manage collections
- **Add to Playlist**: Quick dropdown to add any song to existing playlists
- **Your Library**: Access all your created playlists in one place

### ❤️ Personal Features
- **Liked Songs**: Heart your favorite tracks with persistent storage and quick access
- **Recently Played**: Track your listening history (last 50 songs)
- **User Profiles**: Dynamic user profiles with real-time music statistics
- **Listening Analytics**: Estimated listening time based on play history
- **Music Activity Stats**: Live counts of liked songs, playlists, and recently played tracks
- **Account Management**: User authentication with secure login/signup

### 🎨 User Experience
- **Dark/Light Theme**: Toggle between themes with user preference persistence
- **Responsive Design**: Fully optimized for desktop, tablet, and mobile devices
- **Clean Interface**: Modern UI with smooth transitions, hover effects, and loading states
- **Adaptive Navigation**: Collapsible sidebar that adapts to screen size and user preference
- **Error Handling**: Graceful error messages with user-friendly feedback
- **Loading States**: Visual feedback during data loading and audio buffering

## 🛠️ Tech Stack

### Frontend
- **React.js 18** - Modern React with Hooks and Context API
- **React Router DOM** - Client-side routing with protected routes
- **Context API** - Global state management (Audio, Auth, Playlist, Likes)
- **Tailwind CSS** - Utility-first CSS framework with custom components
- **Shadcn/ui** - High-quality, accessible component library
- **Lucide React** - Beautiful, customizable icon library
- **Vite** - Fast development server and build tool

### Backend & Data Management
- **JSON Server** - RESTful API simulation with full CRUD operations
- **Axios** - HTTP client for API requests with error handling
- **LocalStorage** - Client-side persistence for user preferences and authentication
- **File System** - Local audio file management and serving

### Development & Build Tools
- **Vite** - Lightning-fast build tool and development server
- **ESLint** - Code linting and formatting with custom rules
- **PostCSS** - CSS processing with Tailwind CSS integration
- **Git** - Version control with collaborative workflow

## 📁 Project Structure

```
RhythmicTunes/
├── my-project/
│   ├── public/
│   │   └──audio/          # Audio files
│   │  
│   ├── src/
│   │   ├── components/     # Reusable components
│   │   │   ├── ui/         # Shadcn/ui 
│   │   │   ├── AudioPlayer.jsx
│   │   │   ├── SongList.jsx
│   │   │   ├── Layout.jsx
│   │   │   └── ...
│   │   ├── contexts/       # React Context 
│   │   │   ├── AudioContext.jsx
│   │   │   ├── AuthContext.jsx
│   │   │   ├── PlaylistContext.jsx
│   │   │   └── LikeContext.jsx
│   │   ├── pages/          # Page components
│   │   │   ├── HomePage.jsx
│   │   │   ├── Browse.jsx
│   │   │   ├── Artists.jsx
│   │   │   ├── Search.jsx
│   │   │   └── ...
│   │   ├── services/       # API services
│   │   │   ├── api.js
│   │   │   ├── musicService.js
│   │   │   └── userService.js
│   │   └── App.jsx
│   ├── db.json            # JSON Server database
│   └── package.json
└── README.md
```

## 🚀 Getting Started

### Prerequisites
- Node.js (v16 or higher)
- npm or yarn

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/AkmalMohammed-1/RhythmicTunes.git
   cd RhythmicTunes/my-project
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Start the JSON Server (Backend)**
   ```bash
   npm run server
   ```
   The API will be available at `http://localhost:3001`

4. **Start the Development Server (Frontend)**
   ```bash
   npm run dev
   ```
   The app will be available at `http://localhost:5173`

### Available Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run server` - Start JSON Server backend
- `npm run lint` - Run ESLint
- `npm run preview` - Preview production build

## 🎯 Usage

1. **Sign Up/Login**: Create an account or login to access the app
2. **Browse Music**: Explore the homepage for popular and recently added songs
3. **Discover Artists**: Visit the Artists page to explore your favorite musicians
4. **Search**: Use the search functionality to find specific songs or artists
5. **Create Playlists**: Build custom playlists from the sidebar
6. **Like Songs**: Heart your favorite tracks for quick access
7. **Control Playback**: Use the bottom audio player for full music control

## 🎯 Key Features in Detail

### Audio System
- **Smart Queue Management**: Intelligent playlist system where clicking play on any song creates a queue from the current context (playlist, browse section, artist songs)
- **Seamless Playback**: Continuous audio playback across page navigation with persistent player state
- **Global Audio Context**: Centralized audio state management with real-time updates across the entire application
- **Advanced Controls**: Full-featured player with shuffle, repeat modes, volume control, and seek functionality
- **Error Handling**: Robust audio error management with user-friendly feedback and retry mechanisms

### Authentication & User Management
- **Secure Authentication**: Protected routes with JWT-like authentication system
- **Persistent Sessions**: Automatic login persistence across browser sessions
- **User Preferences**: Theme settings, volume levels, and personalization options
- **Profile Analytics**: Real-time tracking of music activity and listening statistics

### Data Management
- **Local Storage Integration**: Efficient client-side data persistence for likes and preferences
- **API Integration**: RESTful API communication with proper error handling
- **Real-time Updates**: Dynamic data synchronization across components and contexts
- **Optimistic UI Updates**: Immediate UI feedback while background operations complete

### Responsive Design & Accessibility
- **Mobile-First Approach**: Fully optimized user experience for mobile devices with touch-friendly interfaces
- **Adaptive Sidebar**: Intelligent sidebar that collapses on mobile and adapts to screen size
- **Touch-Optimized Controls**: Large, accessible touch targets for mobile music control
- **Cross-Device Compatibility**: Consistent experience across desktop, tablet, and mobile platforms
- **Performance Optimized**: Fast loading times and smooth animations on all device types
- **Accessibility Features**: ARIA labels, keyboard navigation, and screen reader support

## 🔧 Configuration

### Environment Variables
Create a `.env` file in the `my-project` directory:
```env
VITE_API_BASE_URL=http://localhost:3001
```

### Theme Configuration
The app supports both light and dark themes. Theme preference is automatically saved and restored.

## 🙏 Acknowledgments

- **Shadcn/ui** for the beautiful component library
- **Lucide** for the comprehensive icon set
- **Tailwind CSS** for the utility-first CSS framework
- **React Team** for the amazing React.js library

⭐ **Star this repository if you found it helpful!**
