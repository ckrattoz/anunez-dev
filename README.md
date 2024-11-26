# anunez.dev - Personal Website

This repository contains the source code for my personal website [anunez.dev](https://anunez.dev), built using **Astro** and **Vue 3**. It’s a platform to showcase my projects, share ideas, and provide resources for the developer community.

## 🚀 Features

- **Astro** for lightning-fast static site generation.
- **Vue 3** integration for dynamic and interactive components.
- **TailWind** Rapidly build modern websites without ever leaving your HTML.
- Responsive design with modern web standards.
- Easy deployment and scalability.

## 📦 Installation

1. Clone this repository:

   ```bash
   git clone https://github.com/ckrattoz/anunez-dev.git
   cd anunez-dev
   ```

2. Install the dependencies:

   ```bash
   npm install
   ```

## 🛠️ Development

To start the development server, run:

```bash
npm run dev
```

This will launch the Astro development server and hot-reload any changes you make.

## ⚙️ Using Vue 3 in Astro

Astro allows you to integrate Vue 3 components seamlessly. To create a Vue component:

1. Add a new Vue file in the `src/components` directory, for example, `HelloWorld.vue`:

   ```vue
   <template>
     <div>
       <h1>Hello from Vue!</h1>
     </div>
   </template>

   <script setup>
   // Add your Vue logic here
   </script>
   ```

2. Import and use your Vue component in an Astro page or layout:

   ```astro
   ---
   import HelloWorld from '../components/HelloWorld.vue';
   ---

   <html>
     <body>
       <HelloWorld />
     </body>
   </html>
   ```

## 🧪 Build for Production

To build your site for production:

```bash
npm run build
```

The static files will be output to the `dist/` directory, ready for deployment.

## 🚀 Deployment

Astro generates static files that can be deployed to any hosting service, such as:

- **Vercel**
- **Netlify**
- **GitHub Pages**

You can configure deployment by following the guides in the [Astro Deployment Documentation](https://docs.astro.build/en/guides/deploy/).

## 📚 Resources

- [Astro Documentation](https://docs.astro.build)
- [Vue 3 Documentation](https://vuejs.org/)
- [Tailwind Documentation](https://tailwindcss.com/)
- [Astro + Vue 3 Guide](https://docs.astro.build/en/guides/integrations-guide/vue/)
- [Astro + Tailwind Guide](https://docs.astro.build/en/guides/integrations-guide/tailwind/)

Feel free to contribute or open issues if you have suggestions to improve the site! 🎉
