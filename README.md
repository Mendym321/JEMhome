# JEM Website Redesign

A modern, responsive website redesign for Jewish Educational Media (JEM) featuring a freemium business model and 5,000+ video archive.

## 🎯 Live Demo

Simply open `index.html` in your browser to see the site!

## 📁 Project Structure

```
jem-website/
├── index.html                  # Main homepage (use jem-homepage-final.html)
├── video-player.html           # Video watch page
├── films.html                  # Films category page
├── articles.html               # Articles library
├── browse-by-date.html         # Timeline navigation
├── search-results.html         # Search page with mixed content
├── topic-passover.html         # Topic page example
├── mixed-content-example.html  # Design reference
└── README.md                   # This file
```

## ✨ Key Features

### Homepage
- **Hero slider** with 3 rotating featured videos (auto-advance every 5 seconds)
- **Mega-menu navigation** (Browse by Type, Topic, Year)
- **4-column responsive grid** (looks perfect on all screens)
- **Beginner banner** (dismissible, appears after first video row)
- **Compact membership banner** with modal popup
- **Clean, professional design** with gold & navy color scheme

### Content Discovery
- **Browse by Type**: Films, Talks, Farbrengens, Dollars, 770 Moments
- **Browse by Topic**: Holidays, Family, Education, Leadership, Spirituality
- **Browse by Year**: Chronological timeline (1950s-1990s)
- **Search**: Mixed content results (videos + articles) with filter tabs
- **Articles Library**: Essays, interviews, news, and written content

### Freemium Model
- **Free Tier**: Videos under 12 min, intro content, 720p
- **Premium ($8/mo)**: All content, 4K, downloads, transcripts
- **Annual ($80/yr)**: Premium + save $16/year
- **Special pricing**: Students/seniors 50% off

## 🎨 Design System

### Colors
- **Primary**: Dark Navy (`#1a1a2e`)
- **Accent**: Gold (`#c9a961`)
- **Free Badge**: Green (`#059669`)
- **Article Badge**: Purple (`#8b5cf6`)

### Typography
- **Headlines**: Playfair Display (serif, elegant)
- **Body**: IBM Plex Sans (clean, readable)

### Components
- Video cards with hover effects
- Article cards with purple border
- Mega-menu dropdowns
- Modal popups
- Dismissible banners
- Pricing cards

## 🚀 Getting Started

### Option 1: Local Viewing
1. Download all files
2. Open `index.html` in your browser
3. That's it! No build process needed.

### Option 2: GitHub Pages (Free Hosting!)
1. Create a GitHub account (if you don't have one)
2. Create a new repository called `jem-website`
3. Upload all files
4. Go to Settings → Pages
5. Select "main" branch as source
6. Your site will be live at: `https://yourusername.github.io/jem-website/`

## 📄 Page Descriptions

### **index.html** (Homepage)
The main landing page featuring:
- Hero slider with 3 rotating videos
- Beginner-friendly banner (appears after first row)
- Featured videos grid (4 columns)
- Recently added videos
- Compact membership banner with modal
- Full navigation system

**File to use**: Rename `jem-homepage-final.html` to `index.html`

### **video-player.html**
Individual video watch page with:
- Video player area
- 4 tabs: Description, Transcript, Related Article, Discussion
- Related videos sidebar
- Action buttons (Like, Save, Share, Download)
- Upgrade prompts for premium content

### **films.html**
Category browsing page showing:
- Breadcrumb navigation
- Filter dropdowns (Duration, Language, Sort)
- Grid/List view toggle
- Video cards with free/premium indicators
- Pagination

**File to use**: Rename `jem-films-page.html` to `films.html`

### **articles.html**
Written content library featuring:
- Featured article showcase
- Category filters (Interviews, Essays, News)
- Article grid with thumbnails
- Sidebar (Most Read, Topics, Newsletter)
- Read time estimates

**File to use**: Rename `jem-articles-page.html` to `articles.html`

### **browse-by-date.html**
Chronological navigation with:
- Decade timeline (1950s-1990s)
- Year cards showing video counts
- Historical context for each period
- Sticky navigation

**File to use**: Rename `jem-browse-by-date.html` to `browse-by-date.html`

### **search-results.html**
Search page with mixed content:
- Filter tabs (All, Videos, Articles)
- Mixed grid with visual differentiation
- Working filter functionality
- Result counts

### **topic-passover.html**
Example topic page showing:
- Topic header with icon
- Breadcrumb navigation
- All Passover-related content
- Mix of videos and articles (if applicable)

## 🔧 Customization

### Change Colors
Edit the CSS variables in any HTML file:
```css
:root {
    --primary: #1a1a2e;        /* Dark navy */
    --accent: #c9a961;         /* Gold */
    --free-color: #059669;     /* Green */
    --article-color: #8b5cf6;  /* Purple */
}
```

### Add Your Own Content
Replace placeholder content:
- Video thumbnails: Update `background: linear-gradient(...)` styles
- Titles and descriptions: Edit text in HTML
- Video counts: Update numbers in navigation
- Links: Point to your actual pages/videos

### Modify Slider Speed
In the JavaScript section, change:
```javascript
setInterval(() => {
    changeSlide(1);
}, 5000);  // ← Change 5000 to desired milliseconds
```

## 🎯 User Flows

### New Visitor Flow
1. Lands on homepage → sees hero slider
2. Notices "New to the Rebbe?" banner after scrolling
3. Clicks "Watch Introduction Video"
4. Views free content
5. Sees membership benefits
6. May sign up or continue browsing

### Topic Browser Flow
1. Hovers "Browse by Topic" in header
2. Clicks "Passover"
3. Views all Passover content
4. Uses filters if needed
5. Watches videos or reads articles

### Researcher Flow
1. Uses search bar
2. Gets mixed results (videos + articles)
3. Filters by content type if desired
4. Finds exactly what they need

## 📱 Responsive Design

The site works beautifully on:
- **Desktop** (1600px+): Full 4-column layout
- **Laptop** (1400px): 3-column layout
- **Tablet** (1000px): 2-column layout
- **Mobile** (640px): Single column

## 🆘 Troubleshooting

### Slider not working?
- Make sure JavaScript is enabled in your browser
- Check browser console for errors (F12)

### Modal not opening?
- Check that `id="membership-modal"` exists
- Verify JavaScript functions are included

### Layout looks weird?
- Clear browser cache (Ctrl+F5 or Cmd+Shift+R)
- Try a different browser
- Check that CSS is loading properly

## 🚧 Future Enhancements

- [ ] User authentication system
- [ ] Payment integration (Stripe)
- [ ] Real video player integration
- [ ] Backend API for content management
- [ ] Advanced search with filters
- [ ] User playlists and favorites
- [ ] Email newsletter system
- [ ] Analytics integration

## 📊 File Sizes

All files are lightweight and optimized:
- HTML files: ~50-150KB each
- No external dependencies except Google Fonts
- Total project size: < 1MB

## 🤝 Contributing

This is a design mockup. To make it production-ready:
1. Set up a backend (Node.js, Python, PHP, etc.)
2. Integrate video hosting (Vimeo, custom CDN)
3. Add payment processing (Stripe, PayPal)
4. Implement user authentication
5. Connect to CMS for content management

## 📝 License

[Your License Here]

## 📧 Contact

For questions about this design:
- Email: [your-email]
- Website: [your-website]

---

**Built with ❤️ for JEM's mission of preserving and sharing the Rebbe's teachings.**

## 🎓 Learning Notes

This project demonstrates:
- Responsive CSS Grid layouts
- CSS custom properties (variables)
- Modal popup patterns
- Mega-menu navigation
- Hero slider implementation
- Freemium business model UI
- Content differentiation (videos vs articles)
- Progressive disclosure (banners, modals)
- Accessible design patterns
