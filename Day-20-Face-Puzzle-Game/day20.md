## Day 20 — Face Puzzle Game

### What I Built
A complete face puzzle game built as a single HTML file 
using Claude — no frameworks, no external dependencies, 
no manual coding.

### Features Generated
- Live webcam capture using getUserMedia()
- Puzzle difficulty selector (3×3, 4×4, 5×5)
- Drag and drop + touch gesture controls
- Piece snap-to-grid with correct position detection
- Live timer (mm:ss format) and move counter
- Win detection with results overlay
- Top 5 leaderboard saved to localStorage
- Retake Photo, Play Again, New Photo buttons
- Mobile responsive design

### My Results
| Difficulty | Time | Moves |
|------------|------|-------|
| 3×3 | [5:09] | [234] |
| 4×4 | [8:00] | [545] |

### Technical Highlights
- Single self-contained HTML file (~500+ lines)
- All CSS and JS inline — zero external dependencies
- Works on Chrome, Firefox, and Safari
- Camera permission denied handled gracefully
- Touch events supported for mobile gameplay

### Key Learnings
- Claude can generate complete interactive browser games 
  from a single detailed prompt
- Webcam access, canvas manipulation, drag-and-drop, and 
  localStorage — all in one file with no frameworks
- Detailed technical requirements in the prompt = 
  production-ready output
- High effort level produces significantly more complete 
  and polished code than Low effort
- Single-file HTML games are extremely portable — 
  works offline, no server needed