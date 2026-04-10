# Persona 3 UI Package

A plug-and-play UI component library derived from the Persona 3 inspired React app. It gives your project a sleek, highly animated aesthetic.

## Requirements

This UI requires Framer Motion for the smooth interface physics and animations:
```bash
npm install framer-motion react-router-dom
```

## Setup Instructions

1. **Drop it in:** Copy this entire folder (`persona-ui/`) into your target project's `src` directory.
2. **Add the Google Font:** The visual style heavily relies on the `Anton` font for its jagged and striking appearance. Add this to your `public/index.html` (for Vite/CRA) or your base layout file (for Next.js):
```html
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Anton&display=swap" rel="stylesheet">
```

## Quick Start Usage

Wrap your page routes or contents with `<PageTransition />` and use the `<P3Menu />` for navigation natively! You can modify `ITEMS` within `P3Menu.jsx` to match your own routes.

```jsx
import { P3Menu, PageTransition } from './persona-ui';

export default function MyAwesomeHackathonApp() {
  return (
    <PageTransition variant="default">
      <P3Menu onNavigate={(page) => console.log('Heading to:', page)} />
    </PageTransition>
  );
}
```
