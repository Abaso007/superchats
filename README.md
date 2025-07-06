# 🚀 ERA by VYNECT™

**ERA** is a premium JavaScript library for **secure, ethical WhatsApp automation and testing** using direct socket communication. Designed for businesses and developers who demand **speed, control, and simplicity**.

---

## 💡 Key Features

- Direct socket connection (no browser)
- Fast and reliable message automation
- Media sending and receiving
- Modular and scalable architecture
- Built for professional and ethical use cases

> ⚠️ **Important:** ERA is strictly intended for **development, testing, and professional use only**, fully compliant with **WhatsApp's Terms of Service**.

---

## 🛠 Installation

```bash
npm install era-bot
```

---

## 🚀 Revolutionary Quick Start Example (Simplified)

```javascript
import ERA from 'era-bot';

// Create session and start instantly
const client = await ERA.start('YOUR_LICENSE_KEY');

// Send a message (text, image, button, video, audio, document, sticker)
client.send({
  to: '+1234567890',
  type: 'text', // Options: text, image, button, video, audio, document, sticker
  content: 'Hello! Welcome to ERA.'
});

// Listen to multiple events in a single block
client.onEvent((event) => {
  const { from, body, type } = event;

  console.log(`Event Type: ${type}, From: ${from}, Message: ${body}`);

  if (type === 'message' && body.toLowerCase() === 'hi') {
    client.send({ to: from, type: 'text', content: 'Hey! How can I help you today?' });
  }

  if (type === 'message' && body.toLowerCase() === 'photo') {
    client.send({ to: from, type: 'image', content: 'https://via.placeholder.com/300', caption: 'photo caption' });
  }

  if (type === 'status') {
    console.log(`Status update from ${from}: ${body}`);
  }

  if (type === 'call') {
    console.log(`Incoming call from ${from}`);
  }

  // Automatic webhook forwarding
  client.webhook('https://yourserver.com/webhook', event);
});
```

➡️ **What makes this revolutionary?**
- **ERA.start()** for instant simplified session
- Unified **client.send()** with flexible message type selection
- Single **onEvent()** handler for all event types
- Built-in **webhook()** function for effortless automation
- No need for complex configuration or multiple listeners

---

## 📄 License

This product is **commercial and licensed** by **VYNECT™**. All rights reserved.

For commercial licensing, please visit: [vynect.com/era](https://vynect.com/era)

---

## 🌐 About VYNECT™

**VYNECT™** builds next-generation automation and digital solutions focused on **speed, connectivity, and innovation**.

Learn more: [vynect.com](https://vynect.com)

---

🚀 **The new ERA documentation is coming soon!**  
📘 **Stay tuned at:** [vynect.com/era](https://vynect.com/era)
