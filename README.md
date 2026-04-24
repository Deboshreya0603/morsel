🥗 Morsel — every bite, better

A smart food coaching web app that helps individuals make better food choices and build healthier eating habits using contextual data, AI insights, and behavioral nudges.


✨ What is Morsel?
Morsel is a single-file, zero-dependency smart nutrition coach built as a responsive web app. It combines real-time contextual awareness (time of day, weather, meal timing) with an AI-powered coaching engine to guide users toward healthier eating — one meal at a time.
No app store. No install. Just open the HTML file in any browser and it works.

🚀 Live Demo

GitHub Pages: https://deboshreya0603.github.io/morsel


📸 Features
🏠 Today Dashboard

Personalized hero card — greets you by name with live time, day, and local weather context
Calorie & macro tracker — visual progress bars for protein, carbs, fats, and fiber
Meal log — log breakfast, lunch, dinner, and snacks with timestamps
Smart insights panel — 4 contextual cards including fiber alerts, streak wins, weekly behavioral patterns, and heat/season tips
Dinner suggestions — 4 meal cards filtered by remaining calories, nutritional gaps, and local cuisine

🤖 AI Coach

Full conversational chat interface powered by Claude (claude-sonnet-4)
Pre-loaded with your nutritional context (calories eaten, macro gaps, streak, location)
Quick-chip shortcuts for common questions — tonight's dinner, weekly analysis, protein tips, meal plans
Responses are warm, practical, and India-cuisine aware

📅 History

Weekly score grid — colour-coded daily health scores (green = good, amber = okay, gray = missed)
Meal history log — past meals with calorie counts, macros, and scores

👤 Profile

Personal goals with progress tracking (weight, protein, fiber)
Diet preferences — vegetarian/vegan/non-veg toggle
Cuisine preferences, allergy flags, activity level

🌙 Dark / Light Mode

One-click theme toggle in the navbar
Preference saved to localStorage — persists across sessions
Full dark palette with deep charcoal surfaces and softened semantic colors


🛠️ Tech Stack
LayerTechnologyFrontendVanilla HTML, CSS, JavaScriptFontsFraunces (serif display) + DM Sans (body) via Google FontsAI EngineAnthropic Claude API (claude-sonnet-4)HostingStatic — any web host, GitHub Pages, Netlify, VercelStoragelocalStorage for theme preferenceDependenciesZero — no frameworks, no npm, no build step

📁 Project Structure
morsel/
├── index.html      # Entire app — HTML + CSS + JS in one file
└── README.md       # This file

⚙️ Setup & Deployment
Run locally
Just open index.html in any modern browser. No server needed.
bashgit clone https://github.com/Deboshreya0603/morsel.git
cd morsel
open index.html   # macOS
# or double-click index.html on Windows/Linux
Deploy to GitHub Pages (free)

Push index.html to your repo
Go to Settings → Pages
Set source to Deploy from branch → main
Your app is live at https://deboshreya0603.github.io/morsel

Deploy to Netlify (free, drag & drop)

Go to netlify.com/drop
Drag and drop the index.html file
Instant live URL — no account needed

Deploy to Vercel (free)
bashnpm i -g vercel
vercel --prod

🤖 AI Configuration
The AI Coach uses the Anthropic Claude API. The system prompt is pre-loaded with:

User profile (name, age, diet type, location, cuisine preferences)
Daily nutritional goals (calories, protein, carbs, fat, fiber)
Today's food log and remaining macros
Contextual signals (time of day, weather, streak data)

To use your own Anthropic API key, the app is configured to call:
POST https://api.anthropic.com/v1/messages
Model: claude-sonnet-4-20250514

Note: The API key must be handled server-side or via a proxy in production to avoid exposing it in the browser. For personal/demo use, the app works with the Anthropic Claude.ai embedded API access.


🎨 Design Philosophy
Morsel is designed to feel warm and human, not clinical or data-heavy:

Typography: Fraunces (editorial serif) paired with DM Sans (clean body) — chosen to feel nourishing, not corporate
Color palette: Teal as the primary action color, amber for caution, coral for alerts — semantic and consistent
Dark mode: Deep charcoal surfaces (#0f0f0e) with full semantic color remapping
Motion: Subtle fade-in page transitions and message animations
No generic AI aesthetics — no purple gradients, no Inter font, no cookie-cutter layouts


🗺️ Roadmap

 Barcode scanner for packaged food logging
 Weekly meal plan generator
 Water intake tracker with reminders
 Integration with fitness trackers (steps → calorie adjustment)
 Multi-user support with cloud sync
 Regional cuisine databases (South Indian, Bengali, Gujarati, etc.)
 Voice input for meal logging


🙏 Acknowledgements

Built with Claude by Anthropic
Fonts by Google Fonts
Inspired by the everyday challenge of eating well in a busy world


📄 License
MIT License — free to use, modify, and deploy.
