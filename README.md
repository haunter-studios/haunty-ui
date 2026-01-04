# Haunty
Hunty is an open-source gamified Web3 platform for creating, playing, and rewarding competitive hunts on Stellar. It enables users to participate in interactive challenges, compete on transparent leaderboards, and earn on-chain rewards through secure wallet authentication — making it ideal for blockchain-powered competitions, community engagement, and learn-to-earn experiences.

## Features
- **Create & Play Hunts**: Users can create, publish, and participate in custom hunt games.
- **Leaderboard**: Track top performers and foster competition.
- **Wallet Integration**: Secure authentication and reward claiming via crypto wallets.
- **Rewards System**: Distribute prizes to winners based on game outcomes.
- **Responsive UI**: Modern, accessible interface with reusable components.

## Tech Stack
- **Framework**: [Next.js](https://nextjs.org/) (React, TypeScript)
- **Styling**: CSS Modules, PostCSS
- **Wallet/Blockchain**: Integrated wallet modal for crypto authentication (see `WalletModal.tsx`)
- **Other**: Modular component design, utility libraries

## Getting Started

1. **Install dependencies:**
   ```bash
   npm install
   # or
yarn install
   ```

2. **Run the development server:**
   ```bash
   npm run dev
   # or
yarn dev
   ```

3. **Open your browser:**
   Visit [http://localhost:3000](http://localhost:3000) to use Hunty.

## Project Structure
- `app/` - Main application logic and pages
- `components/` - UI and logic components (games, leaderboard, wallet, rewards)
- `lib/` - Utility functions and shared logic
- `public/` - Static assets (images, icons)

## Contributing
Contributions are welcome! Please open an issue or submit a pull request for any improvements or bug fixes.

## License
This project is licensed under the MIT License. See `LICENSE` for details.