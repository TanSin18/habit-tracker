# Discipline Tracker

A beautiful, gamified habit tracking PWA that turns self-improvement into a rewarding journey. Built with React and designed for real behavioral change.

![Version](https://img.shields.io/badge/version-5.0-purple)
![PWA](https://img.shields.io/badge/PWA-Ready-green)
![License](https://img.shields.io/badge/license-MIT-blue)

---

## The Problem

Most habit trackers fail because they're boring. You check a box, nothing happens, and you forget about it by day 3. There's no consequence for failure and no reward for success.

## The Solution

Discipline Tracker gamifies habit building with:
- **Real financial stakes** - Earn rewards for consistency, face penalties for slacking
- **Tiered scoring system** - Weekly performance ratings from Crisis to Elite
- **Visual progress** - Heatmaps, streaks, and achievement badges
- **Smart insights** - Analytics that reveal your patterns

---

## Features

### Core Tracking
- **16 customizable habits** across categories (health, productivity, mindfulness)
- **Daily scoring** with weighted points based on habit difficulty
- **Weekly tier system** - Elite (94+), Solid (83+), Decent (70+), Struggling (55+), Crisis
- **Streak tracking** with longest streak records

### Gamification
- **Achievement badges** - 20+ unlockable achievements for milestones
- **Guilt-Free Fund** - Earn money for hitting targets, spend guilt-free
- **Streak Freezes** - Buy protection for sick days (50 points each)
- **Weekly rewards/penalties** - Real consequences drive real change

### Analytics & Insights
- **Best day detection** - Discover which day you perform best
- **Habit completion rates** - See your strongest and weakest habits
- **Weekly trend charts** - Visualize your progress over time
- **35-day heatmap** - GitHub-style contribution graph

### Data & Sync
- **GitHub Gist sync** - Free cloud backup with full version history
- **Offline-first** - Works without internet, syncs when connected
- **Export/Import** - Download JSON backups anytime
- **Conflict resolution** - Smart handling of multi-device edits

### Mobile Experience
- **PWA** - Install as native app on any device
- **Responsive design** - Optimized for mobile-first usage
- **Haptic feedback** - Tactile responses for interactions
- **Swipe navigation** - Gesture-based week navigation

---

## Tech Stack

| Layer | Technology |
|-------|------------|
| **Frontend** | React 18 (CDN) |
| **Styling** | Tailwind CSS |
| **Storage** | localStorage + GitHub Gist API |
| **PWA** | Service Worker + Web App Manifest |
| **Transpilation** | Babel Standalone |
| **Deployment** | GitHub Pages |

### Architecture Highlights

- **Single HTML file** - Zero build process, instant deployment
- **Offline-first** - Service worker caches for offline use
- **Debounced sync** - Efficient API usage (2s debounce)
- **Error boundary** - Graceful crash recovery with data export
- **Version migration** - Automatic data schema upgrades

---

## Screenshots

### Daily View
Track today's habits with instant feedback and scoring.

### Weekly Overview
See your entire week at a glance with the heatmap.

### Insights Dashboard
Discover patterns in your behavior with analytics.

### Achievements
Unlock badges as you hit milestones.

---

## Quick Start

### Option 1: Use Hosted Version
Visit the live app at your GitHub Pages URL.

### Option 2: Run Locally
```bash
# Clone the repo
git clone https://github.com/TanSin18/habit-tracker.git

# Open in browser (no build needed!)
open index.html
```

### Option 3: Deploy Your Own
1. Fork this repository
2. Enable GitHub Pages (Settings → Pages → Source: main)
3. Access at `https://yourusername.github.io/habit-tracker`

---

## Setting Up Cloud Sync

1. Click **"Connect"** in the app footer
2. Create a GitHub Personal Access Token with `gist` scope
3. Paste the token and connect
4. Your data now syncs to a private Gist automatically

**Benefits:**
- Free unlimited storage
- Full revision history (every save is versioned)
- Access from any device
- You own your data

---

## The Scoring System

### Daily Points
| Habit | Points | Category |
|-------|--------|----------|
| Home-cooked Meals | 2 each | Health |
| Gym/Training | 1 | Fitness |
| Reading | 1-20 (tiered) | Growth |
| Meditation | 1 | Mindfulness |
| Journaling | 1 | Reflection |
| Career Development | 1 | Growth |
| Sleep Tracking | 1 | Health |
| And more... | | |

### Weekly Tiers
| Tier | Score | Reward/Penalty |
|------|-------|----------------|
| Elite | 94+ | +₹100 |
| Solid | 83+ | +₹60 |
| Decent | 70+ | +₹30 |
| Struggling | 55+ | -₹75 |
| Crisis | <55 | -₹200 |

---

## Project Structure

```
habit-tracker/
├── index.html      # Complete app (React + styles + logic)
├── manifest.json   # PWA manifest for installability
├── sw.js          # Service worker for offline support
└── README.md      # This file
```

---

## Key Learnings

Building this project taught me:

1. **Gamification psychology** - How rewards, streaks, and social proof drive behavior
2. **Offline-first architecture** - Service workers, caching strategies, sync conflicts
3. **Single-file deployment** - Shipping without a build process
4. **GitHub API integration** - Using Gists as a free database
5. **PWA best practices** - Manifest, service worker, installability

---

## Future Roadmap

- [ ] Social accountability (share progress with friends)
- [ ] Custom habit creation
- [ ] Weekly email digests
- [ ] Data visualization exports
- [ ] Habit correlation analysis

---

## Contributing

Contributions welcome! Feel free to:
- Report bugs
- Suggest features
- Submit pull requests

---

## License

MIT License - feel free to use this for your own habit tracking journey.

---

## Acknowledgments

Built with discipline, for discipline.

*"We are what we repeatedly do. Excellence, then, is not an act, but a habit."* — Aristotle

---

<p align="center">
  <strong>Start tracking. Start winning.</strong>
</p>
