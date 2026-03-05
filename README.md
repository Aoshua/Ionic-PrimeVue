# IonicPrimeVue

A project combining [Ionic Framework](https://ionicframework.com/), [PrimeVue](https://primevue.org/), and [Tailwind CSS](https://tailwindcss.com/).

---

## Prerequisites

Install the Ionic CLI globally:

```bash
npm install -g @ionic/cli
```

## Project Setup

This project was scaffolded with:

```bash
ionic start
```

---

## PrimeVue

### Install

```bash
npm install primevue @primeuix/themes
```

### Configure

Add PrimeVue to `main.ts`:

```ts
import { createApp } from "vue"
import PrimeVue from "primevue/config"
import Aura from "@primeuix/themes/aura"

const app = createApp(App)
app.use(PrimeVue, {
	theme: {
		preset: Aura
	}
})
```

---

## Tailwind CSS

### Install

```bash
npm install tailwindcss @tailwindcss/vite
```

### Configure Vite

Add the Tailwind plugin to `vite.config.ts`:

```ts
import { defineConfig } from "vite"
import tailwindcss from "@tailwindcss/vite"

export default defineConfig({
	plugins: [tailwindcss()]
})
```

### Add CSS Imports

In your CSS file (e.g. `variables.css`):

```css
@import "tailwindcss";
@import "tailwindcss-primeui";
```

### Add a native iOS and Android project using Capacitor:

```bash
ionic capacitor add
```
