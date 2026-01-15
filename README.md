# Haunty
Hunty is an open-source gamified Web3 platform for creating, playing, and rewarding competitive hunts on Stellar. It enables users to participate in interactive challenges, compete on transparent leaderboards, and earn on-chain rewards through secure wallet authentication — making it ideal for blockchain-powered competitions, community engagement, and learn-to-earn experiences.

## Features
- **Create & Play Hunts**: Users can create, publish, and participate in custom hunt games.
- **Leaderboard**: Track top performers and foster competition.
- **Wallet Integration**: Secure authentication and reward claiming via crypto wallets.
- **Rewards System**: Distribute prizes to winners based on game outcomes.
- **Responsive UI**: Modern, accessible interface with reusable components.

## Tech Stack
- **Framework**: [Next.js](https://nextjs.org/) (React, TypeScript) with App Router
- **Styling**: Tailwind CSS v4, PostCSS, Radix UI primitives
- **State Management**: React hooks with prop drilling (for now)
- **UI Components**: Custom components built with Radix UI primitives
- **Icons**: Lucide React for scalable vector icons
- **Form Handling**: React controlled components
- **Wallet Integration**: Simulated wallet connect (ready for real wallet SDK integration)

## Getting Started

1. **Install dependencies:**
   ```bash
   pnpm install
   # or
   npm install
   # or
   yarn install
   ```

2. **Run the development server:**
   ```bash
   pnpm run dev
   # or
   npm run dev
   # or
   yarn dev
   ```

3. **Open your browser:**
   Visit [http://localhost:3000](http://localhost:3000) to use Hunty.

## Project Structure
```
hunty/
├── app/                    # Next.js App Router
│   ├── hunty/             # Game creator and player interface
│   │   └── page.tsx       # Main game creation/play interface
│   ├── layout.tsx         # Root layout with font configuration
│   └── page.tsx           # Landing page
│
├── components/            # Reusable UI components
│   ├── CreateGameTabs.tsx # Creation flow tabs
│   ├── GameCompleteModal.tsx
│   ├── GamePreview.tsx
│   ├── Header.tsx         # Top navigation with wallet
│   ├── HuntCards.tsx      # Interactive game cards
│   ├── HuntForm.tsx       # Hunt creation form
│   ├── LeaderBoardTable.tsx
│   ├── PlayGame.tsx       # Game runtime
│   ├── PublishModal.tsx
│   ├── RewardsPanel.tsx
│   ├── WalletModal.tsx
│   ├── icons/             # Custom SVG icons
│   └── ui/                # Primitive UI components
│
├── lib/                   # Utilities and configurations
│   ├── font.ts           # Google Fonts setup
│   └── utils.ts          # Helper functions
│
└── public/               # Static assets
    ├── icons/            # App icons
    └── static-images/    # Default images
```

## How It Works

### Game Creation Flow
1. **Create Hunts**
   - Add multiple hunt cards with titles, descriptions, and unlock codes
   - Optionally include images or links for each hunt
   - Set up rewards for top performers

2. **Preview & Test**
   - Real-time preview of how hunts will appear
   - Test the game flow before publishing
   - Validate unlock codes and progression

3. **Publish & Share**
   - Publish hunts for others to play
   - Share game links with participants
   - Monitor leaderboard standings

### Gameplay Experience
- Players progress through a series of hunt cards
- Each card presents a challenge or question
- Correct unlock codes reveal the next challenge
- Completion time and accuracy determine leaderboard position

## Architecture

### Key Components
- **State Management**: Component-level state with prop drilling (consider Zustand/Context for larger scale)
- **UI Layer**: Built with Radix UI primitives and Tailwind CSS
- **Game Logic**: Client-side validation and progression tracking
- **Wallet Integration**: Ready for Web3 wallet connection

### Data Flow
1. User creates hunts → State updates in `app/hunty/page.tsx`
2. Preview renders via `GamePreview` component
3. Play mode uses `PlayGame` and `HuntCards` for the interactive experience
4. Completion triggers `GameCompleteModal` with leaderboard options

## Development

### Prerequisites
- Node.js ^18.16.0
- pnpm
- Modern browser with ES2020+ support

### Available Scripts
```bash
# Install dependencies
pnpm install

# Run development server
pnpm dev

# Build for production
pnpm build

# Start production server
pnpm start

# Lint code
pnpm lint
```

## Contributing

We welcome contributions! Here's how to get started:

1. **Fork** the repository and create a feature branch
2. **Install** dependencies with `pnpm install`
3. **Make** your changes following the code style
4. **Test** your changes thoroughly
5. **Commit** with a clear message
6. **Push** to your fork and open a Pull Request


## License
This project is licensed under the MIT License. See `LICENSE` for details.