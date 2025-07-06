# 🚀 ERA by VYNECT™

**ERA** is a premium JavaScript library for **secure, ethical WhatsApp automation and testing** using direct socket communication. Designed for businesses and developers who demand **speed, control, and reliability**.

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

## 🚀 Revolutionary Quick Start Example

```javascript
import { createSession } from 'era-bot';

(async () => {
  const client = await createSession({
    sessionName: 'vynect-session',
    license: 'YOUR_LICENSE_KEY'
  });

  const actions = {
    hello: async (msg) => await msg.reply('Hi! Welcome to the future of messaging.'),
    photo: async (msg) => await msg.sendImage(
      'https://via.placeholder.com/300',
      'photo',
      'Here is your requested photo.'
    ),
    bye: async (msg) => await msg.reply('Goodbye! See you soon.')
  };

  client.autoHandle(actions);
})();
```

➡️ **What makes this revolutionary?**
- Declarative **autoHandle()** with action mapping
- No need for manual `if` conditions
- Clean, scalable, instantly maintainable code

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
