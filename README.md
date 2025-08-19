# Diet Consultant App – Beginner’s GitHub Guide 🚀

Welcome! This step-by-step guide will help you (even if you’re totally new to GitHub) set up your Diet Consultant App repository and get started.

---

## 1. Create Your GitHub Account

- Go to [github.com](https://github.com)
- Click **Sign up**
- Enter your email, create a password, and choose a username (e.g., `DietAppPro`)
- Verify your email

---

## 2. Create Your First Repository

- After logging in, click the **+** icon (top-right) → **New repository**
- Name it: `diet-consultant-app`
- Description: `My awesome diet app for Chandigarh clients!`
- Check **Add a README file**
- Click **Create repository**

---

## 3. Add Your First Files

### a) Create folder structure

- Click **Add file** → **Create new file**
- Type `backend/.env.example` in the filename box
- Paste this:

    ```
    # Database settings
    DATABASE_URL="postgresql://user:password@localhost:5432/dietdb"
    ```

- Click **Commit new file**

### b) Add frontend file

- Click **Add file** → **Create new file**
- Type `frontend/pages/index.js` in the filename box
- Paste this:

    ```jsx
    export default function Home() {
      return (
        <div>
          <h1>Welcome to My Diet App!</h1>
          <p>Healthy eating starts here 🥗</p>
        </div>
      )
    }
    ```

- Click **Commit new file**

---

## 4. Clone to Your Computer (Where Magic Happens ✨)

- Install [GitHub Desktop](https://desktop.github.com/) (easiest way)
- Log in with your GitHub account
- Click **Clone repository** → Select `diet-consultant-app`
- Choose where to save it (e.g., `Documents/GitHub`)

---

## 5. Add More Files Locally

- Open the folder in [VS Code](https://code.visualstudio.com/)
- Create these files:

### `backend/prisma/schema.prisma`

```prisma
datasource db {
  provider = "postgresql"
  url      = env("DATABASE_URL")
}

model User {
  id    Int     @id @default(autoincrement())
  email String  @unique
  name  String?
}
```

### `frontend/components/LandingPage.jsx`

```jsx
export default function LandingPage() {
  return (
    <div className="bg-green-100 p-8">
      <h1 className="text-3xl font-bold">Personalized Diet Plans</h1>
      <button className="bg-blue-500 text-white px-4 py-2 mt-4">
        Get Started
      </button>
    </div>
  )
}
```

---

## 6. Save Changes to GitHub

- In GitHub Desktop:
    - You’ll see your changes listed
    - Write a summary like `Added basic files`
    - Click **Commit to main**
    - Click **Push origin** to send to GitHub

---

## 7. See Your Live Website! 🌐

- Go to [vercel.com](https://vercel.com/)
- Sign in with GitHub
- Click **Add New** → **Project**
- Select your repository
- Click **Deploy**
- Your app will be live at `diet-consultant-app.vercel.app`!

---

## 8. Next Steps to Build Your App

Open VS Code terminal and run:

```bash
cd frontend
npm install next react react-dom
npm run dev
```

---

**You’re all set!**  
If you need help, check out [GitHub Docs](https://docs.github.com/) or ask your mentor.
# diet-consultant-app
App DeepSeek 
