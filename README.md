# 🚀 3D Developer Portfolio

A modern, interactive developer portfolio featuring stunning 3D visuals, smooth animations, and a responsive design. Built with React, Three.js, and cutting-edge web technologies to showcase your skills in the most engaging way possible.

![Portfolio Preview](https://images.unsplash.com/photo-1618005182384-a83a8bd57fbe?w=1200&h=600&fit=crop)

## ✨ Features

### 🎨 **Visual Excellence**

- **Interactive 3D Scene** - Floating geometric objects with real-time lighting and shadows
- **Smooth Animations** - Framer Motion powered transitions and micro-interactions
- **Modern Dark Theme** - Beautiful purple/violet accent colors with professional styling
- **Responsive Design** - Flawlessly adapts to all screen sizes and devices

### 🛠 **Technical Highlights**

- **Performance Optimized** - Efficient rendering with React Three Fiber
- **Accessibility First** - WCAG compliant with proper ARIA labels and keyboard navigation
- **SEO Ready** - Structured data and meta tags for optimal search engine visibility
- **Type Safety** - Full TypeScript implementation for robust development

### 📱 **User Experience**

- **Smooth Scrolling** - Seamless navigation between sections
- **Mobile Responsive** - Touch-friendly interactions and mobile-optimized layouts
- **Fast Loading** - Optimized assets and efficient code splitting
- **Cross-browser Compatible** - Works flawlessly across all modern browsers

## 🎯 Sections

- **Hero** - Eye-catching introduction with animated call-to-actions
- **About** - Personal story, experience highlights, and key strengths
- **Skills** - Categorized technology showcase with animated reveals
- **Projects** - Featured work with live demos and source code links
- **Contact** - Professional contact form and social media integration

## 🛠 Tech Stack

### **Frontend**

- [React 18](https://reactjs.org/) - Modern UI library with latest features
- [TypeScript](https://www.typescriptlang.org/) - Type-safe JavaScript
- [Vite](https://vitejs.dev/) - Lightning-fast build tool and dev server
- [React Router 6](https://reactrouter.com/) - Client-side routing

### **3D Graphics & Animation**

- [Three.js](https://threejs.org/) - 3D graphics library
- [React Three Fiber](https://github.com/pmndrs/react-three-fiber) - React renderer for Three.js
- [React Three Drei](https://github.com/pmndrs/drei) - Useful helpers for R3F
- [Framer Motion](https://www.framer.com/motion/) - Production-ready motion library

### **Styling & UI**

- [TailwindCSS 3](https://tailwindcss.com/) - Utility-first CSS framework
- [Radix UI](https://www.radix-ui.com/) - Unstyled, accessible UI components
- [Lucide React](https://lucide.dev/) - Beautiful & consistent icon library
- [Class Variance Authority](https://cva.style/) - Type-safe component variants

### **Backend & API**

- [Express.js](https://expressjs.com/) - Fast, unopinionated web framework
- [Zod](https://zod.dev/) - TypeScript-first schema validation

### **Development Tools**

- [Vitest](https://vitest.dev/) - Fast unit testing framework
- [ESLint](https://eslint.org/) - Code linting and formatting
- [Prettier](https://prettier.io/) - Code formatting

## 🚀 Quick Start

### Prerequisites

- Node.js 18+
- npm, yarn, or pnpm

### Installation

1. **Clone the repository**

   ```bash
   git clone https://github.com/yourusername/3d-portfolio.git
   cd 3d-portfolio
   ```

2. **Install dependencies**

   ```bash
   npm install
   # or
   yarn install
   # or
   pnpm install
   ```

3. **Start the development server**

   ```bash
   npm run dev
   ```

4. **Open your browser**
   Navigate to `http://localhost:8080` to see your portfolio in action!

## 📁 Project Structure

```
├── client/                    # Frontend React application
│   ├── components/
│   │   ├── 3d/               # Three.js components
│   │   │   └── Scene.tsx     # Main 3D scene
│   │   ├── portfolio/        # Portfolio sections
│   │   │   ├── Navigation.tsx
│   │   │   ├── Hero.tsx
│   │   │   ├── About.tsx
│   │   │   ├── Skills.tsx
│   │   │   ├── Projects.tsx
│   │   │   └── Footer.tsx
│   │   └── ui/               # Reusable UI components
│   ├── pages/                # Route components
│   │   ├── Index.tsx         # Homepage
│   │   └── NotFound.tsx      # 404 page
│   ├── lib/                  # Utility functions
│   ├── hooks/                # Custom React hooks
│   ├── App.tsx               # App entry point
│   └── global.css            # Global styles
├── server/                   # Express.js backend
│   ├── routes/               # API route handlers
│   └── index.ts              # Server configuration
├── shared/                   # Shared types and utilities
└── public/                   # Static assets
```

## 🎨 Customization Guide

### **Colors & Theme**

Update the color scheme in `client/global.css`:

```css
:root {
  --primary: 262 80% 60%; /* Purple accent */
  --background: 222 47% 5%; /* Dark background */
  --foreground: 210 40% 98%; /* Light text */
  /* Add your custom colors here */
}
```

### **3D Scene**

Modify the 3D elements in `client/components/3d/Scene.tsx`:

- Add new geometric shapes
- Adjust lighting and materials
- Change animation speeds
- Customize camera positions

### **Content**

Update your personal information in:

- `client/components/portfolio/Hero.tsx` - Name, title, bio
- `client/components/portfolio/About.tsx` - Experience, stats
- `client/components/portfolio/Skills.tsx` - Technologies
- `client/components/portfolio/Projects.tsx` - Portfolio projects

### **Animations**

Customize animations in any component using Framer Motion:

```tsx
<motion.div
  initial={{ opacity: 0, y: 20 }}
  animate={{ opacity: 1, y: 0 }}
  transition={{ duration: 0.8 }}
>
  Your content
</motion.div>
```

## 🚢 Deployment

### **Build for Production**

```bash
npm run build
```

### **Start Production Server**

```bash
npm start
```

### **Deploy to Vercel**

1. Connect your GitHub repository to Vercel
2. Configure build settings:
   - Build Command: `npm run build`
   - Output Directory: `dist/spa`
3. Deploy!

### **Deploy to Netlify**

1. Build your project: `npm run build`
2. Upload the `dist/spa` folder to Netlify
3. Configure redirects for SPA routing

### **Docker Deployment**

```bash
# Build the Docker image
docker build -t portfolio .

# Run the container
docker run -p 3000:3000 portfolio
```

## 🔧 Development

### **Available Scripts**

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run start` - Start production server
- `npm test` - Run tests
- `npm run typecheck` - Check TypeScript types
- `npm run format.fix` - Format code with Prettier

### **Adding New API Routes**

1. Create route handler in `server/routes/`
2. Register route in `server/index.ts`
3. Add types in `shared/api.ts`

### **Adding New Pages**

1. Create component in `client/pages/`
2. Add route in `client/App.tsx`

## 🎯 Performance Tips

- **3D Optimization**: Use `useFrame` sparingly and optimize geometries
- **Image Optimization**: Use WebP format and proper sizing
- **Code Splitting**: Lazy load components with `React.lazy()`
- **Bundle Analysis**: Use `npm run build -- --analyze` to inspect bundle size

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- **Three.js Community** - For the amazing 3D graphics library
- **React Three Fiber** - For making Three.js React-friendly
- **Radix UI** - For accessible, unstyled components
- **Tailwind CSS** - For the utility-first styling approach
- **Framer Motion** - For beautiful, performant animations

## 📬 Contact

Feel free to reach out if you have any questions or suggestions!

- **Portfolio**: [Your Portfolio URL]
- **Email**: mburukiganya@gmil.com
- **LinkedIn**: https://www.linkedin.com/in/kiganya-mburu-53a7b5231/
- **Twitter**: https://x.com/kiganyamburu

---


