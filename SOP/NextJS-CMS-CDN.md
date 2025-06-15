## NextJS CMS-CDN (
Ref: https://nextjs.org/learn
Ref: https://nextjs.org/learn/react-foundations
Ref: https://github.com/vercel/next-learn/tree/main/dashboard/starter-example
- Next.js is an open-source React-based  framework used for building server-side rendering (SSR) web applications.
- It provides an efficient and easy-to-use environment for developing web applications with minimal setup and configuration.
- Full-stack starters, SaaS starter, Cloud-ready starters, Backend starters, Landing page starters, eCommerce starters,

## Create project. 
- Package manager pnpm faster and more efficient than npm or yarn
- npm install -g pnpm 
- npx create-next-app@latest nextjs-dashboard --example "https://github.com/vercel/next-learn/tree/main/dashboard/starter-example" --use-pnpm
- Run pnpm i to install the project's packages.
- Run pnpm dev to start the development server.
- Visit http://localhost:3000

### CSS Styling
- Tailwind is a CSS framework that speeds up the development process by allowing you to quickly write utility classes directly in your React code.
- Two different ways of styling: Tailwind and CSS modules.
- Add global styles to your application by navigating to /app/layout.tsx and importing the global.css file

### Optimizing Fonts and Images
- With fonts, layout shift happens when the browser initially renders text in a fallback or system font and then swaps it out for a custom font once it has loaded. This swap can cause the text size, spacing, or layout to change, shifting elements around it.
- Import the Inter font from the next/font/google module - this will be your primary font. Then, specify what subset you'd like to load. In this case, 'latin':
- /app/ui folder, create a new file called fonts.ts
- Finally, add the font to the <body> element in /app/layout.tsx:

### Creating Layouts and Pages
- Routing: Next.js uses file-system routing where folders are used to create nested routes. Each folder represents a route segment that maps to a URL segment.
- You can create separate UIs for each route using layout.tsx and page.tsx files.
- The /app/page.tsx - this is the home page associated with the route /.
- Similarly /app/dashboard/page.tsx is associated with the /dashboard path
- Only the content inside the page file will be publicly accessible. For example, the /ui and /lib folders are colocated inside the /app folder along with your routes.

-  ./openssl rand -base64 32
-  http://localhost:3000/seed
