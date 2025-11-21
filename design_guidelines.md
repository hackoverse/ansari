# Business Trading Platform - Design Guidelines

## Design Approach
**Reference-Based Strategy**: Drawing inspiration from Airbnb's marketplace sophistication, Stripe's professional restraint, Linear's modern SaaS aesthetics, and SMERGERS' business-focused interface. Create a premium, trustworthy platform that balances professional credibility with engaging user experience.

## Typography System
- **Primary Font**: Inter (via Google Fonts) - clean, professional, excellent at all sizes
- **Display Font**: Space Grotesk (via Google Fonts) - bold headers and hero text
- **Hierarchy**:
  - Hero headlines: text-5xl to text-7xl, font-bold, Space Grotesk
  - Section headers: text-3xl to text-4xl, font-semibold
  - Card titles: text-xl, font-semibold
  - Body text: text-base, regular weight
  - Metadata/labels: text-sm, font-medium
  - Captions: text-xs, text-gray-600

## Layout System
**Spacing Primitives**: Use Tailwind units of 2, 4, 6, 8, 12, 16, 20, 24 for consistent rhythm
- Section padding: py-20 (desktop), py-12 (mobile)
- Card padding: p-6 to p-8
- Container max-widths: max-w-7xl for full sections, max-w-4xl for content
- Grid gaps: gap-6 to gap-8

## Component Library

### Navigation
- **Desktop Header**: Sticky top navigation with logo left, main menu center, CTA buttons right (Login/Signup, Sell Business)
- **Mobile**: Hamburger menu with slide-in drawer, prominent search icon
- Add trust badge: "10,000+ Verified Businesses" in header

### Hero Section (Home)
- Full-width hero: min-h-[600px] with gradient overlay on background image
- Centered content with large headline (text-6xl), subheading, dual CTA buttons
- Integrated search bar with category dropdown, location input, voice search icon
- Floating trust indicators: "500+ Deals Closed", "₹100Cr+ Transactions"

### Business Cards
- **Grid Layout**: grid-cols-1 md:grid-cols-2 lg:grid-cols-3, gap-6
- **Card Structure**:
  - Image area: aspect-video with overlay badge (Featured/AI Recommended)
  - Content section: Business name (text-xl), industry tag, location
  - Key metrics row: Revenue, Profit, Established year (icons + numbers)
  - Price badge: Prominent, top-right or bottom
  - Hover effect: Subtle lift (shadow-lg), smooth transition

### Filter Sidebar (Explore Page)
- Left sidebar: w-80, sticky positioning
- Collapsible filter groups: Industry, Location, Price Range, Turnover, Employees
- Multi-select checkboxes with count badges
- Range sliders for price/revenue
- Clear filters button at bottom

### Business Detail Page
- **Layout**: Two-column on desktop (2/3 content, 1/3 sidebar)
- **Hero**: Full-width image gallery (carousel with thumbnails)
- **Tabbed Interface**: Overview, Financials, Documents, AI Insights, Similar Businesses
- **Sidebar**: Sticky contact card with seller info, price, enquiry form, save/share buttons
- **AI Section**: Distinct visual treatment with gradient border, summary cards, risk score badge

### Messaging Interface
- **Split Layout**: Conversation list (1/3) + active chat (2/3)
- Message bubbles: Rounded, sender right/receiver left, timestamps
- Input bar: File attachment, voice note, send button
- Video/audio call buttons in header

### Dashboard Cards
- **Grid**: grid-cols-1 md:grid-cols-2 lg:grid-cols-4 for metrics
- **Stat Cards**: Icon, large number, label, trend indicator (up/down arrow)
- **Activity Feed**: Timeline layout with avatar, action, timestamp

### Forms
- Floating label inputs with focus states
- Multi-step form for listing creation with progress indicator
- File upload: Drag-drop zone with preview thumbnails
- Inline validation with icon indicators

### Admin Panel
- **Sidebar Navigation**: Fixed left, icon + label, active state highlight
- **Data Tables**: Sortable columns, action dropdowns, pagination
- **Analytics**: Chart.js integration for graphs, metric cards dashboard

## Micro-Interactions
- **Button States**: Subtle scale on hover (scale-105), active press effect
- **Card Hovers**: Lift effect with shadow transition
- **Loading**: Skeleton screens for content, spinner for actions
- **Search**: Auto-suggest dropdown with category grouping
- Keep animations minimal and purposeful - avoid excessive motion

## Icons
**Library**: Heroicons via CDN (outline for general use, solid for emphasis)
- Navigation: home, search, chat, user icons
- Filters: funnel, location-marker, currency icons
- Actions: heart (save), share, phone, video-camera
- Status: check-circle (verified), exclamation (alert)

## Images Section

### Hero Image (Home Page)
Large hero background image (1920x800px): Professional business handshake or modern office setting with subtle blur/overlay for text readability. Position behind hero content with gradient overlay from transparent to dark.

### Business Listing Images
- Thumbnail images: aspect-video (16:9), minimum 800x450px
- Gallery images: High-resolution business premises, team photos, product images
- Placeholder: Professional generic business imagery when seller hasn't uploaded

### Category Cards
Industry-specific imagery: Restaurant interior, IT office workspace, manufacturing floor, retail storefront - use as card backgrounds with overlay

### Profile/Avatar Images
- Circular avatars (w-12 h-12) for sellers, chat participants
- Default: Initials on gradient background when no photo

### AI Features Illustrations
Abstract, modern illustrations for AI sections - use SVG graphics from Undraw or similar for: chatbot interface, analytics dashboard, document scanning

## Unique Visual Elements
- **Glass-morphism**: Backdrop blur for overlays, floating cards (backdrop-blur-sm)
- **Gradient Accents**: Subtle gradients on CTA buttons, feature cards
- **Badge System**: Industry tags, verification badges, trending indicators
- **Trust Signals**: Verified checkmarks, security badges, testimonial cards with photos
- **Rich Tooltips**: Hover tooltips with additional context on metrics/terms

## Responsive Breakpoints
- Mobile-first approach
- Breakpoints: sm (640px), md (768px), lg (1024px), xl (1280px)
- Stack columns on mobile, expand to multi-column on md+
- Touch-friendly tap targets (min 44x44px) on mobile

This creates a premium, AI-enhanced marketplace that feels modern, trustworthy, and engaging while maintaining professional credibility essential for business transactions.