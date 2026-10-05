# Live Streaming Admin Panel — Complete Specification

## 1. Project Goal

Build a complete, production-ready Admin Management Panel for a Live Streaming / Social Audio & Video application.

Use the provided reference screenshots as the primary UI/UX inspiration for:

- Sidebar structure
- Dashboard layout
- Statistic cards
- Header
- Search
- Spacing
- Colors
- Typography
- Tables
- Admin controls

Do not blindly copy branding or copyrighted assets. Recreate the professional dashboard structure with original implementation and assets.

The panel must be scalable, responsive, secure, and ready to connect to a real backend/API.

---

# 2. Recommended Technology

## Frontend

- React
- TypeScript
- Vite
- Tailwind CSS
- shadcn/ui or equivalent reusable components
- Lucide React icons
- React Router
- TanStack Query
- Recharts
- React Hook Form
- Zod

## Backend Ready Architecture

Prepare the frontend for:

- REST API
- WebSocket / real-time updates
- Authentication
- Role-Based Access Control
- Database
- Pagination
- Search
- Sorting
- Filtering
- File uploads
- Audit logs

## Suggested Folder Structure

```text
src/
├── components/
├── pages/
├── layouts/
├── routes/
├── hooks/
├── services/
├── api/
├── types/
├── utils/
├── lib/
├── assets/
└── config/
```

---

# 3. Main Admin Layout

Create a professional desktop-first admin dashboard.

## Left Sidebar

The sidebar should be fixed on desktop and collapsible.

### Top

- App logo
- App name
- Quick Find
- Menu search
- Keyboard shortcut: Ctrl + K

### Main Navigation

1. Dashboard
2. Team Performance
3. Wallet History
4. Users
5. Top Up
6. Store
7. VIP
8. Beans Packages
9. Gifts
10. Stickers
11. Notifications
12. Transactions
13. Content
14. Live Streaming
15. My Badge
16. Spot Light
17. Host Rewards
18. Daily Star
19. User Host Level
20. Onboard
21. Games
22. Settings
23. Logs
24. Support

Every navigation item must have:

- Icon
- Label
- Active state
- Hover state
- Optional expand arrow
- Permission check
- Working route

---

# 4. Top Header

Create a sticky top header.

## Left

- Breadcrumb
- Current page title

## Quick Navigation

- Users
- Hosts
- Search

## Right

- Filter icon
- Messages icon
- Notification bell
- Admin profile

Example profile:

```text
Official Management
Administrator
```

Profile dropdown:

- My Profile
- Account Settings
- Security
- Activity
- Logout

---

# 5. Dashboard

Create an Administrator Overview dashboard.

Header:

```text
ADMINISTRATOR OVERVIEW

Dashboard
```

Show:

- Live data indicator
- Last update time
- Auto-refresh information

Example:

```text
Live data
Live counts refresh every 45 seconds
```

---

# 6. Main Statistics Cards

Create responsive statistic cards.

## Cards

### Platform Users

Example:

```text
2,453
Platform users
```

### VIP Subscribers

```text
0
VIP subscribers
```

### Store Beans Sold

```text
460,578
Store beans sold
```

### Withdraw Volume

```text
0
Withdraw volume
```

Each card should contain:

- Icon
- Large number
- Label
- Optional trend
- Optional percentage
- Hover animation
- Clickable navigation

---

# 7. Global Search

Create a large search panel.

Placeholder:

```text
Search users, hosts, codes...
```

Search button:

```text
Search
```

Search should support:

- Users
- Hosts
- User ID
- Host ID
- Username
- Phone
- Email
- Agency
- Referral code
- Gift code
- Transaction ID
- Withdrawal ID

Search results should show:

- Avatar
- Name
- ID
- Type
- Status
- Balance
- Host status
- Actions

---

# 8. Quick Metrics

Create Quick Metrics cards.

## Required Cards

1. Wallet
2. Pending Withdrawals
3. Support Chats
4. VIP Subscribers
5. Administrators
6. Admin
7. Agencies
8. Developer
9. Golden Top Up
10. Country Head
11. Hosts
12. Top Up Agents
13. Users
14. Blocked
15. Coins Clean
16. Coins Record
17. Game P/L (7d)

Each card should link to its related management page.

---

# 9. Dashboard Action Cards

Create large cards for:

## Golden Top-up Beans

Example:

```text
186,000

View agents →
```

## Pending Withdrawals

Example:

```text
0

Review transactions →
```

## New Registrations Today

Example:

```text
945

Browse users →
```

---

# 10. Users Management

Create a complete Users management page.

## Sections

- All Users
- Active Users
- Blocked Users
- Banned Users
- New Users
- VIP Users
- Hosts
- Agents

## Table Columns

- Avatar
- User ID
- Username
- Name
- Country
- Phone
- Email
- Coins
- Beans
- VIP Level
- Host Status
- Account Status
- Registration Date
- Last Active
- Actions

## Actions

- View
- Edit
- Block
- Unblock
- Ban
- Unban
- Delete
- Reset Password
- Add Coins
- Remove Coins
- Add Beans
- View Wallet
- View Transactions
- View Live History

## Required Features

- Search
- Filters
- Sorting
- Pagination
- Bulk actions
- CSV export

---

# 11. Host Management

Create Host Management.

## Sections

- All Hosts
- Active Hosts
- Offline Hosts
- Pending Hosts
- Suspended Hosts
- Top Hosts
- Host Applications

## Host Data

- Host ID
- Name
- Username
- Country
- Agency
- Level
- Followers
- Total Live Hours
- Viewers
- Gifts Received
- Beans Earned
- Revenue
- Host Status

## Actions

- Approve
- Reject
- Suspend
- Activate
- Edit
- View Profile
- View Live History
- View Earnings
- Assign Agency
- Change Host Level

---

# 12. Live Streaming Management

Create a real-time Live Streaming management page.

## Live Room Data

- Room ID
- Host
- Title
- Category
- Country
- Viewers
- Duration
- Gifts
- Coins
- Status

## Actions

- Watch Live
- View Room
- Mute
- Warn Host
- End Stream
- Ban User
- Remove User
- Send Announcement
- Manage Moderators

## Live Room Detail

Show:

- Live video preview
- Host information
- Viewer list
- Live chat
- Gifts
- Moderators
- Reports
- Room settings
- Activity log

---

# 13. Team Performance

Create Team Performance dashboard.

Show:

- Total Agents
- Active Agents
- New Users
- Active Hosts
- Host Performance
- Revenue
- Beans
- Coins
- Top Performing Team Members

## Charts

- Daily Registrations
- Host Activity
- Revenue
- Beans
- Coins
- Live Hours

## Date Filters

- Today
- Yesterday
- 7 Days
- 30 Days
- Custom Range

---

# 14. Wallet History

Create wallet transaction history.

## Columns

- User
- User ID
- Transaction ID
- Type
- Coins
- Beans
- Amount
- Balance Before
- Balance After
- Date
- Status

## Filters

- User
- Transaction Type
- Date
- Amount
- Status

---

# 15. Top Up Management

Create Top Up management.

## Sections

- Top Up Orders
- Top Up Agents
- Golden Top Up
- Top Up Codes
- Pending Top Ups
- Completed
- Failed

## Data

- Order ID
- User
- Agent
- Amount
- Coins
- Payment Method
- Status
- Date

## Actions

- Approve
- Reject
- Refund
- View Details

---

# 16. Store

Create Store management.

## Product Data

- Product Name
- Image
- Price
- Coins
- Stock
- Status

## Actions

- Add Product
- Edit
- Delete
- Activate
- Deactivate
- Manage Inventory

---

# 17. VIP Management

Create VIP system.

## VIP Levels

- Level Name
- Required Coins
- Benefits
- Badge
- Duration
- Status

## Actions

- Add VIP Level
- Edit
- Delete
- Activate
- Deactivate

## VIP Users

Show:

- User
- VIP Level
- Start Date
- Expiry
- Coins Spent
- Status

---

# 18. Beans Packages

Create Beans Package management.

## Fields

- Package Name
- Beans
- Price
- Bonus
- Currency
- Status
- Display Order

## Actions

- Add
- Edit
- Delete
- Activate
- Deactivate

---

# 19. Gifts Management

Create virtual gift management.

## Fields

- Gift Name
- Gift Image
- Animation
- Coin Price
- Beans Value
- Category
- Status

## Actions

- Add Gift
- Edit
- Delete
- Upload Animation
- Activate/Deactivate
- Change Sort Order

---

# 20. Stickers

Create sticker management.

## Features

- Sticker Packs
- Sticker Name
- Image
- Price
- Category
- Status

## Actions

- Add
- Edit
- Delete
- Upload
- Activate
- Deactivate

---

# 21. Notifications

Create notification center.

## Notification Types

- Push Notification
- In-App Notification
- Announcement

## Fields

- Title
- Message
- Image
- Target Audience
- Country
- User Type
- Schedule
- Status

## Target Audience

- All Users
- Hosts
- VIP Users
- Agencies
- Specific Users

---

# 22. Transactions

Create complete transaction management.

## Transaction Types

- Coin Purchase
- Gift Transaction
- Top Up
- Withdrawal
- Refund
- Bonus
- Admin Adjustment
- Host Earning

## Columns

- Transaction ID
- User
- Type
- Amount
- Coins
- Beans
- Payment Method
- Status
- Date

## Actions

- View Details
- Approve
- Reject
- Refund
- Export

---

# 23. Content Management

Create CMS.

## Manage

- Banners
- Announcements
- Posts
- Stories
- Categories
- Featured Content
- Promotional Content

## Actions

- Create
- Edit
- Delete
- Publish
- Unpublish
- Schedule

---

# 24. My Badge

Create Badge Management.

## Fields

- Badge Name
- Badge Icon
- Level
- Requirement
- Description
- Status

Assign badges to:

- Users
- Hosts
- VIP Users

---

# 25. Spot Light

Create Spotlight Management.

## Features

- Featured Hosts
- Featured Users
- Featured Rooms
- Promotion Slots

## Fields

- Name
- Image
- Position
- Start Date
- End Date
- Status

## Actions

- Add
- Edit
- Remove
- Schedule

---

# 26. Host Rewards

Create Host Rewards system.

Rewards can be based on:

- Live Hours
- Viewers
- Gifts
- Beans
- Coins
- Daily Performance
- Weekly Performance
- Monthly Performance

Admin actions:

- Create Reward
- Edit Reward
- Delete Reward
- Approve Reward
- View Reward History

---

# 27. Daily Star

Create Daily Star leaderboard.

Show:

- Top Host
- Top User
- Most Gifts
- Most Viewers
- Most Live Hours
- Most Coins
- Most Beans

Include ranking/leaderboard UI.

---

# 28. User Host Level

Create Host Level management.

## Level Data

- Level Name
- Required Hours
- Required Beans
- Required Viewers
- Benefits
- Badge

## Actions

- Create Level
- Edit
- Delete
- Reorder

---

# 29. Onboarding

Create onboarding management.

## Manage

- New Host Applications
- Agency Applications
- Documents
- Verification
- Approval Status

## Status

- Pending
- Under Review
- Approved
- Rejected

## Actions

- Review
- Approve
- Reject
- Request Documents
- Add Notes

---

# 30. Games

Create Games management.

## Game Data

- Game Name
- Icon
- Category
- Players
- Revenue
- Status

## Actions

- Add Game
- Edit
- Delete
- Activate
- Deactivate
- View Statistics

## Game P/L

Show:

- Daily P/L
- Weekly P/L
- Monthly P/L
- Total Bets
- Total Wins
- Total Losses

---

# 31. Settings

Create complete Settings.

## General

- App Name
- Logo
- Favicon
- Default Language
- Timezone
- Currency

## User Settings

- Registration
- Login
- OTP
- Password Policy
- Account Deletion

## Live Settings

- Maximum Room Users
- Stream Quality
- Recording
- Chat Settings
- Moderation

## Payment Settings

- Payment Gateways
- Coins
- Beans
- Withdraw Settings
- Minimum Withdrawal
- Maximum Withdrawal

## Notification Settings

- Push
- Email
- SMS

## Security

- 2FA
- Login Security
- Session Management
- IP Restrictions
- Rate Limiting
- Admin Permissions

---

# 32. Logs

Create Audit Logs.

Track:

- Admin Login
- Admin Logout
- User Changes
- Host Changes
- Wallet Changes
- Coin Changes
- Bean Changes
- Payment Changes
- Settings Changes
- Deleted Records

## Columns

- Log ID
- Admin
- Action
- Target
- IP
- Device
- Timestamp
- Details

---

# 33. Support

Create Support Center.

## Features

- Support Tickets
- Live Support Chats
- User Complaints
- Host Complaints
- Payment Issues
- Technical Issues

## Statuses

- Open
- Pending
- In Progress
- Resolved
- Closed

## Actions

- Reply
- Assign Ticket
- Add Internal Note
- Close Ticket
- Reopen Ticket

---

# 34. Admin & Role Management

Create Role-Based Admin Management.

## Roles

- Super Admin
- Administrator
- Admin
- Country Head
- Agency Manager
- Host Manager
- Finance Manager
- Support Agent
- Developer

## Permissions

- Dashboard
- Users
- Hosts
- Live Streaming
- Wallet
- Top Up
- Payments
- VIP
- Gifts
- Content
- Games
- Reports
- Settings
- Logs
- Support

Each permission supports:

- View
- Create
- Edit
- Delete
- Approve
- Export

---

# 35. Agency Management

Create Agency Management.

## Fields

- Agency ID
- Agency Name
- Owner
- Country
- Hosts
- Active Hosts
- Total Beans
- Revenue
- Status

## Actions

- Add Agency
- Edit
- Suspend
- Activate
- Assign Hosts
- View Performance

---

# 36. Reports & Analytics

Create an analytics dashboard.

## Charts

- User Growth
- Host Growth
- Live Rooms
- Viewer Growth
- Coins Revenue
- Beans Generated
- Withdrawals
- Top Up
- Gift Revenue
- VIP Subscriptions

## Date Filters

- Today
- 7 Days
- 30 Days
- 3 Months
- 6 Months
- 1 Year
- Custom Date

## Export

- CSV
- Excel
- PDF

---

# 37. Security Requirements

Implement strong security architecture.

Required:

- HTTPS
- Secure Authentication
- JWT/Session Security
- Password Hashing
- Role-Based Access Control
- Permission Checks
- Input Validation
- XSS Protection
- CSRF Protection
- SQL Injection Protection
- Rate Limiting
- Secure File Upload
- File Type Validation
- File Size Validation
- Admin 2FA
- Session Expiration
- Login Attempt Protection
- Audit Logging
- Secure Environment Variables
- Never expose secrets in frontend
- Never expose private API keys

---

# 38. Database Structure

Prepare database models/tables for:

```text
users
admins
roles
permissions
hosts
agencies
wallets
wallet_transactions
coins
beans
topups
topup_agents
withdrawals
vip_levels
vip_subscriptions
beans_packages
gifts
gift_transactions
stickers
notifications
live_rooms
live_viewers
live_messages
live_gifts
host_rewards
badges
spotlights
daily_star
host_levels
onboarding
games
game_transactions
support_tickets
content
reports
audit_logs
settings
```

Every major entity should include:

- id
- created_at
- updated_at
- status

Use proper relationships and indexes.

---

# 39. UI Design

Follow the overall design language of the reference screenshots.

## Colors

Use:

- White/light background
- Soft gray borders
- Purple/blue primary accent
- Green success
- Red danger
- Orange warning
- Subtle gradients where appropriate

## Cards

Cards should include:

- Small colored icon box
- Large number
- Small label
- Optional badge
- Optional trend

## Tables

Tables should include:

- Clean headers
- Sticky header where useful
- Search
- Filters
- Sorting
- Pagination
- Action dropdown

## UX

Use:

- Skeleton loaders
- Empty states
- Error states
- Confirmation modals
- Toast notifications
- Loading indicators
- Accessible form labels

---

# 40. Responsive Design

## Desktop

- Fixed sidebar
- Full dashboard
- Multi-column statistic cards

## Tablet

- Collapsible sidebar
- Responsive cards
- Adaptive tables

## Mobile

- Hamburger menu
- Sidebar drawer
- Responsive cards
- Horizontal table scrolling
- Responsive forms

Never allow content to overflow incorrectly.

---

# 41. Real-Time Architecture

Prepare the system for WebSocket/Supabase Realtime/Firebase-compatible real-time functionality.

Real-time data:

- Online Users
- Live Rooms
- Viewer Count
- Gifts
- Chat
- New Registrations
- Transactions
- Notifications
- Support Chats

Dashboard should display:

```text
Live data
```

and update without requiring a full page refresh.

---

# 42. Performance

Implement:

- Lazy loading
- Code splitting
- Pagination
- Debounced search
- Image optimization
- Cached API requests
- Optimized charts
- Virtualized large lists when required
- Efficient database queries

---

# 43. Environment Variables

Create an `.env.example`.

Example:

```env
VITE_API_BASE_URL=
VITE_WS_URL=
VITE_SUPABASE_URL=
VITE_SUPABASE_ANON_KEY=
VITE_APP_NAME=
VITE_STORAGE_URL=
```

Never commit real secrets.

---

# 44. Routing

Create working routes such as:

```text
/dashboard
/team-performance
/wallet-history
/users
/hosts
/top-up
/store
/vip
/beans-packages
/gifts
/stickers
/notifications
/transactions
/content
/live-streaming
/my-badge
/spotlight
/host-rewards
/daily-star
/user-host-level
/onboard
/games
/settings
/logs
/support
/agencies
/reports
/admins
```

Use protected routes for admin-only pages.

---

# 45. Final Requirements

Do NOT create only a visual mockup.

Create a complete scalable Admin Panel architecture.

Every sidebar option must have:

- Working route
- Page UI
- Search where relevant
- Filters where relevant
- Tables where relevant
- Forms where relevant
- Modals where relevant
- Loading state
- Empty state
- Error state
- Permission checking

All buttons should have meaningful behavior.

All navigation links must work.

All dropdowns must work.

All forms must validate.

All destructive actions must require confirmation.

Use realistic demo data so the dashboard looks populated.

Keep components reusable and maintainable.

The final result should feel like a professional Live Streaming Platform Management System inspired by the supplied reference screenshots.
