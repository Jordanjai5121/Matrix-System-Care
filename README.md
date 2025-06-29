# Matrix System Care Website

A modern, responsive website for Matrix System Care - Mobile & Computer Sales & Service.

## Features

- **Dynamic Routing**: Multi-page application with React Router
- **Responsive Design**: Mobile-first design that works on all devices
- **Matrix Theme**: Futuristic design inspired by the Matrix movie
- **Service Management**: Detailed service pages with dynamic routing
- **Gallery System**: Image gallery with category filtering
- **Contact Forms**: Interactive contact forms with validation
- **Content Management**: Easy-to-update content system

## Project Structure

```
src/
├── components/          # Reusable components
│   ├── Header.tsx      # Navigation header
│   ├── Footer.tsx      # Site footer
│   ├── Layout.tsx      # Page layout wrapper
│   └── MatrixRain.tsx  # Matrix rain animation
├── pages/              # Page components
│   ├── Home.tsx        # Homepage
│   ├── Services.tsx    # Services listing
│   ├── ServiceDetail.tsx # Individual service pages
│   ├── Gallery.tsx     # Image gallery
│   ├── About.tsx       # About page
│   └── Contact.tsx     # Contact page
├── data/               # Content management
│   └── content.ts      # Business data and content
└── App.tsx             # Main app with routing
```

## Adding New Content

### Adding Images to Gallery

1. Place image files in the `public/images/` folder
2. Update the `galleryImages` array in `src/data/content.ts`:

```typescript
{
  id: 7,
  src: '/images/your-image.jpg',
  alt: 'Description of image',
  category: 'Service Category'
}
```

### Adding New Services

1. Add service data to `servicesData` array in `src/data/content.ts`
2. Create detailed service information with features, pricing, etc.

### Updating Business Information

Edit the `businessInfo` object in `src/data/content.ts` to update:
- Contact details
- Address
- Business hours
- Owner information

## Deployment Options

### Option 1: Netlify (Recommended)
1. Build the project: `npm run build`
2. Deploy the `dist` folder to Netlify
3. Set up custom domain if needed

### Option 2: Vercel
1. Connect your GitHub repository to Vercel
2. Vercel will automatically build and deploy

### Option 3: Traditional Web Hosting
1. Run `npm run build`
2. Upload the contents of the `dist` folder to your web server

## Development

```bash
# Install dependencies
npm install

# Start development server
npm run dev

# Build for production
npm run build

# Preview production build
npm run preview
```

## Customization

### Colors and Styling
- Primary colors are defined in Tailwind classes
- Matrix theme uses green (#00ff41), cyan, and blue gradients
- Dark background with neon accents

### Adding New Pages
1. Create new page component in `src/pages/`
2. Add route to `src/App.tsx`
3. Update navigation in `src/components/Header.tsx`

### Content Updates
All business content is centralized in `src/data/content.ts` for easy updates without touching component code.

## Support

For technical support or customization requests, contact the development team.