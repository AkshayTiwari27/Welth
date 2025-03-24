
# **Welth - AI Finance Platform**  
<img width="1470" alt="Screenshot 2024-12-10 at 9 45 45 AM" src="https://github.com/user-attachments/assets/1bc50b85-b421-4122-8ba4-ae68b2b61432">

## **Overview**  
**Welth** is an AI-powered financial management platform designed to help users take control of their finances through **smart budgeting, automated transaction tracking, and insightful financial analysis**. Built with **Next.js, PostgreSQL, and Supabase (with Prisma ORM),** Welth ensures a seamless and secure experience for managing personal and business finances.  

## 🚀 Live Demo  
Experience Welth in action: [Click Here](https://welth-pearl.vercel.app/)

## **Features**  

### **🚀 Modern Landing Page**  
- Engaging **scroll-triggered animations** for a dynamic introduction.  
- Clear **value proposition** with key platform features.  
- **Fully responsive design** for an optimal experience across devices.  

### **📊 Interactive Dashboard**  
- **Secure authentication** with **Clerk** .  
- **Real-time budget tracking** with visual analytics.  
- **Comprehensive transaction overview** with spending insights.  

### **💰 Advanced Transaction Management**  
- **Smart filtering & sorting** for income and expenses.  
- **Automated recurring transactions** for better financial planning.  
- **Bulk transaction management** for effortless data handling.  
- **AI-powered receipt scanning** using **Gemini API** for auto-entry and categorization.  

### **📉 Intelligent Budgeting & AI-Powered Reports**  
- Customizable **budget creation and tracking**.  
- **Automated alerts** for exceeding budget limits.  
- **Monthly AI-generated financial reports** with spending pattern insights.  
- Actionable **recommendations** to optimize financial health.  

---

## **🔧 Technologies Used**  

### **Frontend**  
- **Next.js** → Server-side rendering & static site generation.  
- **Shadcn UI** → Modern UI components for an intuitive experience.  
- **TypeScript** → Static typing for reliability and maintainability.  

### **Backend & Database**  
- **Clerk** → Authentication provider for secure user sign-in.  
- **Supabase (PostgreSQL)** → Scalable, real-time database.  
- **Prisma ORM** → Type-safe database queries & migrations.  
- **Supabase Edge Functions** → Secure serverless functions for financial calculations.  

### **Security & Performance**  
- **Arcjet** → Rate limiting & bot protection for improved security.  

### **AI & Data Processing**  
- **Gemini API** → Reading receipts to automatically add transactions.  
- **Ingest AI** → Receipt data processing and categorization.  

### **Deployment & Hosting**  
- **Vercel** → Optimized performance for Next.js applications.  

---

## **🚀 Setup Instructions**  

### **1️⃣ Clone the Repository**  
```sh
git clone https://github.com/AkshayTiwari27/Welth.git
cd welth
```

### **2️⃣ Install Dependencies**  
```sh
npm install
```

### **3️⃣ Set Up Environment Variables**  
Create a **`.env`** file in the root directory and add the following:  

```
DATABASE_URL=
DIRECT_URL=

NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=
CLERK_SECRET_KEY=
NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up
NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=/onboarding
NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=/onboarding

GEMINI_API_KEY=

RESEND_API_KEY=

ARCJET_KEY=
```


### **4️⃣ Run Database Migrations (Prisma + Supabase)**  
```sh
npx prisma migrate dev
```

### **5️⃣ Run the Development Server**  
```sh
npm run dev
```
- Open **`http://localhost:3000`** to view the app in your browser.  

---

## **🛠 Contribution Guidelines**  

### **1️⃣ Fork the Repository**  
Click the **"Fork"** button to create a copy of the repository under your GitHub account.  

### **2️⃣ Create a Branch**  
```sh
git checkout -b feature/your-feature-name
```

### **3️⃣ Make Your Changes**  
Ensure your code adheres to the **project’s coding standards**.  

### **4️⃣ Commit Your Changes**  
```sh
git commit -m "Add feature: your feature"
```

### **5️⃣ Push Changes & Create a Pull Request**  
```sh
git push origin feature/your-feature-name
```
Submit a **Pull Request (PR)** for review.  

---

## **🗂 Project Architecture**  

```
welth/
│── pages/            # Next.js pages for routing  
│── components/       # Reusable UI components (Shadcn UI)  
│── lib/              # Utility functions, API integrations, and helper functions  
│── public/           # Static assets (images, icons, fonts)  
│── styles/           # Global styles and CSS modules  
│── api/              # Next.js API routes for backend functionality  
│── ai_services/      # AI-powered transaction processing & financial analysis  
│── database/         # Prisma database schema & migrations  
│── auth/             # Clerk authentication logic  
│── security/         # Arcjet-based rate limiting & bot protection  
```

---

## **🛡 Security & Compliance Considerations**  

- **Authentication & Authorization:** Uses **Clerk** for secure sign-in with JWT tokens.  
- **Database Security:** Implements **Supabase Row-Level Security (RLS) and Prisma access controls**.  
- **Encryption:** Transactional data is encrypted to **ensure privacy and compliance with financial regulations**.  
- **Bot Protection:** **Arcjet integration** to mitigate bot attacks and enforce rate limiting.  
- **Compliance Standards:** Ensuring future alignment with **GDPR & PCI DSS** for secure financial data handling.  

---

## **🌟 Future Enhancements**  
- **🔗 Bank & Financial Institution Integrations** (Plaid, Open Banking APIs).  
- **📈 Advanced Investment Tracking & Portfolio Management**.  
- **💡 AI-driven Insights & Personalized Financial Planning**.  
- **🔒 Enhanced Fraud Detection & Security Features**.  

---

## **📜 License**  
This project is licensed under the **MIT License**. See the [LICENSE](./LICENSE) file for details.  

---


