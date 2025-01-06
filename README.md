<!-- markdownlint-disable MD030 -->

# Flowise Embed

Javascript library to display flowise chatbot on your website

Install:

```bash
yarn install
```

Dev:

```bash
yarn dev
```

A development server will be running on http://localhost:5678 automatically. Update `public/index.html` to connect directly to Flowise:

```html
<!-- public/index.html -->
<script type="module">
  import Chatbot from 'https://localhost:5678/web.js'; // Change to from './web.js' to 'https://localhost:5678/web.js'
  Chatbot.init({
    chatflowid: '91e9c803-5169-4db9-8207-3c0915d71c5f', // Add your Flowise chatflowid
    apiHost: 'https://your-flowise-instance.com', // Add your Flowise apiHost
  });
</script>
```

Build:

```bash
yarn build
```

## Custom URL parameters

- `f27_tooltip` : For custom tooltip message
- `f27_welcome_message` : For custom welcome message

## Important

Keep server running while pushing code to github

## Embed in your HTML

### PopUp

```html
<script type="module">
  import Chatbot from 'https://cdn.jsdelivr.net/npm/flowise-embed/dist/web.js';
  Chatbot.init({
    chatflowid: '<chatflowid>',
    apiHost: 'http://localhost:3000',
  });
</script>
```
