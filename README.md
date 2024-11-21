# Titans: Smart Agricultural Land Reclamation & Water Access System  

## **Overview**  
This project addresses food security and water access challenges in Africa through an innovative integration of **blockchain** and **AI** technologies. Built on the **Internet Computer Protocol (ICP)**, the system leverages **Rust** for backend development (smart contracts and APIs) and **React** for creating an interactive and user-friendly frontend interface.  

---

## **Features**  
1. **Land Analysis**:  
   AI-driven insights and recommendations for reclaiming degraded lands efficiently.  
2. **Blockchain-based Land Registry**:  
   Tokenized and secure records of land ownership to enhance transparency and accountability.  
3. **Water Access Management**:  
   Real-time monitoring of borehole usage and a credit-based system for managing water access.  
4. **Crowdfunding Platform**:  
   A blockchain-secured platform for transparent funding of land reclamation and water projects.  

---

## **Tech Stack**  

### **Backend**  
- **Rust**: For implementing ICP canisters (smart contracts).  
- **ICP**: The blockchain infrastructure supporting decentralized storage and execution.  

### **Frontend**  
- **React**: Built with **TypeScript** for robust development.  
- UI Framework: **Material-UI** or **TailwindCSS** for modern design.  
- Deployed as an **asset canister** on the ICP blockchain.  

### **AI Integration**  
- Hosted on external servers and accessed via **ICP HTTP outcalls** for scalability and performance.  

### **Database**  
- **Stable Memory**: For persistent and efficient storage within ICP canisters.  
- **IPFS**: For managing large file storage requirements.  

---

## **Getting Started**  

### **1. Prerequisites**  
Ensure you have the following installed:  
- **Rust**: For building and deploying backend canisters.  
- **Node.js** and **npm**: Required for frontend development.  
- **DFX SDK**: To interact with ICP canisters.  
- A **stable internet connection** for deployment and interaction with the ICP network.  

### **2. Project Structure**  
```plaintext
/project-root
│
├── backend/          # Rust canisters
│   ├── src/          # Rust source files
│   ├── Cargo.toml    # Rust dependencies
│   └── dfx.json      # ICP project configuration
│
├── frontend/         # React app
│   ├── src/          # React source files
│   ├── public/       # Public assets
│   ├── package.json  # React dependencies
│   └── dfx.json      # ICP frontend deployment configuration
│
└── README.md         # Project documentation
```  

---

## **Backend Setup**  

1. **Navigate to the Backend Directory**:  
   ```bash
   cd backend
   ```  

2. **Build Canisters**:  
   Compile the Rust canisters.  
   ```bash
   dfx build
   ```  

3. **Deploy Canisters Locally**:  
   Start the local ICP environment and deploy the canisters.  
   ```bash
   dfx start --background
   dfx deploy
   ```  

4. **Test Canisters**:  
   Invoke methods for testing using the following command:  
   ```bash
   dfx canister call <canister-name> <method-name> '(<arguments>)'
   ```  

---

## **Frontend Setup**  

1. **Navigate to the Frontend Directory**:  
   ```bash
   cd frontend
   ```  

2. **Install Dependencies**:  
   ```bash
   npm install
   ```  

3. **Start Development Server**:  
   Launch the development server for testing.  
   ```bash
   npm start
   ```  

4. **Build and Deploy the Frontend**:  
   - Build the production-ready app:  
     ```bash
     npm run build
     ```  
   - Deploy the frontend as an asset canister:  
     ```bash
     dfx deploy frontend
     ```  

---

## **Running Locally**  

1. **Start the Backend**:  
   ```bash
   dfx start --background
   ```  

2. **Deploy Backend Canisters**:  
   ```bash
   dfx deploy
   ```  

3. **Run the Frontend**:  
   ```bash
   cd frontend
   npm start
   ```  

4. **Access the App**:  
   Visit the app at [http://localhost:8080](http://localhost:8080).  

---

## **Contributing**  
We welcome contributions!  
- **Issues**: Report bugs or propose features via GitHub Issues.  
- **Pull Requests**: Submit enhancements or fixes through PRs.  

---

## **License**  
This project is licensed under the **MIT License**. Refer to the `LICENSE` file for details.  
