<a href="https://portfolio-rdvb.vercel.app"><img align="right" src="./frontend-button.svg" width="140" alt="Live Portfolio" /></a>

### Neel Samel | Developer Portfolio

<em>A responsive portfolio showcasing my work, skills, experience, and ways to get in touch.</em>

<p align="left">
  <img src="https://img.shields.io/badge/Next.js-000000?style=flat&logo=next.js&logoColor=white" alt="Next.js" />
  &nbsp;
  <img src="https://img.shields.io/badge/React-20232A?style=flat&logo=react&logoColor=61DAFB" alt="React" />
  &nbsp;
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=typescript&logoColor=white" alt="TypeScript" />
  &nbsp;
  <img src="https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=flat&logo=tailwindcss&logoColor=white" alt="Tailwind CSS" />
  &nbsp;
  <img src="https://img.shields.io/badge/Framer_Motion-0055FF?style=flat&logo=framer&logoColor=white" alt="Framer Motion" />
  &nbsp;
  <img src="https://img.shields.io/badge/Nodemailer-22A7F0?style=flat&logo=nodemailer&logoColor=white" alt="Nodemailer" />
</p>

<hr />

### 🚀 About the project

**Neel Samel's portfolio** is a responsive web application built with Next.js. It presents my background, skills, experience, and selected projects, and includes a contact form for sending messages. The projects page supports category filtering, text search, and pagination. Visitors can also switch between light and dark themes and access my resume.

### ✨ Features

<table>
  <tr>
    <td valign="top">

- ✅ Responsive portfolio with Home, About, Projects, and Contact sections
- ✅ Profile, skills, services, work experience, and education highlights
- ✅ Project cards with technology tags, source links, and live demos
- ✅ Filter projects by Full Stack, Frontend, and Backend categories
- ✅ Search projects by title and description

</td>
    <td valign="top">

- ✅ Paginated project results
- ✅ Light and dark themes with the selected preference saved locally
- ✅ Theme follows the system preference on first visit
- ✅ Resume viewing and download links
- ✅ Contact form backed by a Next.js API route and Nodemailer

</td>
  </tr>
</table>

### 🛠️ Tech Stack

|             Framework & Language             |         Styling & Animation         |                   UI & Server Utilities                   |
| :------------------------------------------: | :---------------------------------: | :--------------------------------------------------------: |
| Next.js, React, TypeScript                   | Tailwind CSS, Framer Motion         | Heroicons, React Icons, Lucide React, Nodemailer           |

### 📷 Screenshots

Project preview images are included in `public/` and displayed on the Projects page. Standalone screenshots of the portfolio interface are not included.

### 🚀 Getting Started

<table>
  <tr>
    <td valign="top" width="40%">

#### Prerequisites

- **Node.js** 20.9 or later
- **npm**
- A Gmail account and app password if you want the contact form to send email

#### ⚙️ Environment Variables

The contact form uses `EMAIL_USER` and `EMAIL_PASS` to send messages through Gmail. Create a `.env.local` file in the project root:

```env
EMAIL_USER=your-email@gmail.com
EMAIL_PASS=your-gmail-app-password
```

> 💡 Use a Gmail app password rather than your regular account password. Keep these values private; `.env.local` is ignored by Git. The portfolio can be viewed without configuring email, but contact form submissions require these variables.

</td>
    <td valign="top" width="60%">

#### Installation

1. Clone the repository and enter the project directory:

```bash
   git clone https://github.com/NEELSAMEL19/Portfolio.git
   cd Portfolio
```

2. Install dependencies:

```bash
   npm install
```

3. Start the development server:

```bash
   npm run dev
```

4. Open [http://localhost:3000](http://localhost:3000) in your browser.

</td>
  </tr>
</table>

### 📁 Project Structure

```text
Portfolio/
├── app/
│   ├── about/page.tsx          # About section
│   ├── api/contact/
│   │   ├── mailer.ts           # Gmail transport for contact messages
│   │   └── route.ts            # Contact form API endpoint
│   ├── contact/page.tsx        # Contact details and form
│   ├── projects/page.tsx       # Searchable, filterable project listing
│   ├── favicon.ico
│   ├── globals.css             # Global styles and Tailwind theme
│   ├── layout.tsx              # Root layout, navigation, and footer
│   └── page.tsx                # Home page
├── components/
│   ├── projects/
│   │   ├── FilterTabs.tsx
│   │   ├── Pagination.tsx
│   │   ├── ProjectCard.tsx
│   │   ├── ProjectsHeader.tsx
│   │   └── SearchBar.tsx
│   ├── Footer.tsx
│   ├── Hero.tsx
│   └── Navbar.tsx
├── contents/projects.ts        # Project content and links
├── context/ThemeContext.tsx    # Light and dark theme state
├── public/
│   ├── images/                 # Portfolio and project images
│   ├── expense-tracker-card.jpg
│   ├── file.svg
│   ├── globe.svg
│   ├── Neel_Samel_Full_Stack_Developer_Resume.pdf
│   ├── next.svg
│   ├── profile.png
│   ├── takshahub-card.jpg
│   ├── vercel.svg
│   └── window.svg
├── types/index.ts              # Shared TypeScript types
├── utils/animations.ts         # Shared Framer Motion variants
├── bun.lockb
├── eslint.config.mjs
├── frontend-button.svg
├── next.config.ts
├── package-lock.json
├── package.json
├── postcss.config.mjs
├── tsconfig.json
└── README.md
```

### 🔗 Backend API

The contact form is handled by a same-origin Next.js API route. It validates the submitted fields and sends the message to the configured Gmail address using Nodemailer.

| Method   | Endpoint        | Description                                      | Auth Required |
| :------: | --------------- | ------------------------------------------------ | :-----------: |
| `POST`   | `/api/contact`  | Send a contact message (`name`, `email`, `message`) |      No       |

<table>
  <tr>
    <td valign="top" width="50%">

#### 👥 Contributing

Contributions are welcome! Feel free to open an issue or submit a pull request with bug fixes, improvements, or ideas for the portfolio.

</td>
    <td valign="top" width="50%">

#### 📄 License

This project is licensed under the [MIT License](LICENSE).

</td>
  </tr>
</table>


Made with ❤️ by [Neel Samel](https://github.com/NEELSAMEL19)
