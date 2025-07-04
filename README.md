## 📚 React Markdown Q&A Renderer
📝 A lightweight React component for rendering rich Q&A content with Markdown support and Prism-based syntax highlighting.

## 🚀 Features
✅ Markdown parsing with react-markdown
✅ Syntax highlighting using react-syntax-highlighter (Prism themes)
✅ Dynamic heading detection & transformation
✅ Easily customizable themes and styles
✅ Works with Vite, Create React App, Next.js, and more.

## ✨ Preview
<img width="959" alt="image" src="https://github.com/user-attachments/assets/db7a642c-cfe3-438f-a253-2633493da021" />

🛠 Installation
bash
Copy
Edit
npm install react react-markdown react-syntax-highlighter
or

bash
Copy
Edit
yarn add react react-markdown react-syntax-highlighter
## 💻 Usage
Here’s a minimal example of using the Answer component:

jsx
Copy
Edit
import React from "react";
import Answer from "./components/Answer";

export default function App() {
  return (
    <div>
      <Answer 
        ans={`## This is a heading\n\n\`\`\`javascript\nconsole.log("Hello World");\n\`\`\``}
        totalResult={2}
        index={1}
        type="a"
      />
    </div>
  );
}
## 🎨 Customizing code highlighting themes
Change the theme by editing the import in your component:

javascript
Copy
Edit
import { atomDark } from "react-syntax-highlighter/dist/esm/styles/prism/atomDark";
Try other Prism themes like:

javascript
Copy
Edit
import { vscDarkPlus } from "react-syntax-highlighter/dist/esm/styles/prism/vscDarkPlus";
import { solarizedlight } from "react-syntax-highlighter/dist/esm/styles/prism/solarizedlight";
import { okaidia } from "react-syntax-highlighter/dist/esm/styles/prism/okaidia";
Then set it in your component:

jsx
Copy
Edit
<SyntaxHighlighter style={vscDarkPlus} language="javascript">
  {code}
</SyntaxHighlighter>
## 🏗 Project structure
css
Copy
Edit
src/
├── components/
│   └── Answer.jsx
├── helper.js
└── App.jsx
## 🤝 Contributing
Pull requests and discussions are welcome!
If you spot bugs or have ideas for improvements (like more customization, tests, or documentation examples), please open an issue or PR.

## 📜 License
MIT License — free to use, modify, and distribute.

## 🌟 Show your support
If you find this helpful, please ⭐ the repo to help others discover it!

