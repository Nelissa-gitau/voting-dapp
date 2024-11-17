SecurePoll
SecurePoll is a blockchain-powered Decentralized Application (DApp) designed for transparent and tamper-proof voting. It ensures a secure, immutable election process using Ethereum smart contracts and provides a user-friendly interface for voters to participate effortlessly.

Features
Blockchain-Backed Voting: Uses Solidity smart contracts to securely record votes.
Real-Time Results: Displays live vote counts fetched directly from the blockchain.
Secure Wallet Connection: Supports MetaMask for voter authentication and transaction signing.
Responsive UI: Built with React and styled using Tailwind CSS for a seamless user experience.
Single Vote Restriction: Ensures each voter can cast only one vote.
Tech Stack
Smart Contract Development: Solidity
Blockchain Framework: Hardhat
Local Blockchain Testing: Ganache
Frontend Framework: React
Blockchain Interaction: Ethers.js
Styling: Tailwind CSS
Setup Instructions
1. Prerequisites
Ensure you have the following installed:

Node.js
MetaMask browser extension
Ganache
2. Clone the Repository
git clone https://github.com/your-username/SecurePoll.git
cd SecurePoll
3. Install Dependencies
npm install
4. Start Ganache
Open Ganache and create a new workspace.
Add the details of your workspace (e.g., port number, network ID).
5. Deploy Smart Contract
Compile and deploy the smart contract using Hardhat:

npx hardhat compile
npx hardhat run scripts/deploy.js --network ganache
6. Update Contract Address
Copy the deployed contract address from the Hardhat output and update the contract address in your frontend:

const contractAddress = "YOUR_DEPLOYED_CONTRACT_ADDRESS";
7. Start the Frontend
npm start
Usage
Connect Wallet: Open the application and connect your MetaMask wallet.
View Candidates: Browse the list of candidates and their current vote counts.
Cast Your Vote: Enter the candidate’s index and click Vote.
Track Results: Monitor real-time voting results on the dashboard.
Smart Contract
The Voting.sol contract manages:

Candidate Registration: Initializes and displays candidates.
Vote Recording: Logs votes immutably, ensuring transparency.
Session Timing: Restricts voting to a specific time frame.
Testing
To test the smart contract:

Run the following command:
npx hardhat test
Review the output to ensure all test cases pass.
Folder Structure
SecurePoll/
├── contracts/       # Solidity smart contracts
├── scripts/         # Deployment scripts
├── src/             # React frontend source files
│   ├── components/  # Reusable React components
│   ├── pages/       # Application pages
├── public/          # Static files
├── test/            # Smart contract test cases
└── package.json     # Dependencies and scripts
Contributing
Contributions are welcome! To contribute:

Fork the repository.
Create a new branch:
git checkout -b feature-name
Commit your changes:
git commit -m "Description of changes"
Push to your fork and create a pull request.
Acknowledgments
Ethereum and Solidity documentation
Hardhat and Ganache communities
React and Tailwind CSS guides
