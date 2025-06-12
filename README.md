
# pixelbot.ai

Welcome to **pixelbot.ai**, an AI-powered full-stack web development environment in the browser. Built on the open-source project **bolt.diy**, pixelbot.ai allows developers to use their favorite Large Language Models (LLMs) to generate, edit, and manage code collaboratively and intelligently.

This project supports LLMs like OpenAI, Anthropic, Ollama, HuggingFace, LM Studio, Groq, Mistral, DeepSeek, and more. You can even integrate your own provider using the Vercel AI SDK.

> 🔗 GitHub Repository: [https://github.com/arvindgfx1/pixelbot.ai.git](https://github.com/arvindgfx1/pixelbot.ai.git)

---

## Features

- 💡 **AI-powered full-stack coding** in the browser  
- 🌐 **Multi-LLM support** with dynamic API keys and base URLs  
- 🔄 **Terminal integration** with live output from commands  
- ♻️ **Chat history + prompt attachments**  
- 🗃️ **Revert to earlier code versions**  
- ⬇️ **Download project as ZIP**  
- 🐳 **Docker support** for isolated environments  
- 🚀 **Deploy to Netlify**  
- 🔧 **Model prompt customization & performance tuning**

---

## Setup

### Prerequisites

- **Node.js** (LTS version recommended): https://nodejs.org/en/download/  
- **pnpm**: install with  
```bash
npm install -g pnpm
```

---

## Run the Application

### Option 1: Local Setup (Recommended)

1. **Install dependencies**
```bash
pnpm install
```

2. **Start development server**
```bash
pnpm run dev
```

Open [http://localhost:5173](http://localhost:5173)

---

### Option 2: Docker Setup

1. **Install Docker**: https://www.docker.com/

2. **Build the image**
```bash
docker build . --target bolt-ai-development
```

3. **Run the container**
```bash
docker compose --profile development up
```

---

## API Key Configuration

1. Open `http://localhost:5173`  
2. Select an LLM provider from the dropdown  
3. Click the ✏️ (edit) icon to input your API key  
4. Optionally configure **base URL** if using local models like Ollama or LM Studio

---

## Supported Providers

- OpenAI  
- Anthropic (Claude)  
- Ollama  
- HuggingFace  
- LM Studio  
- xAI  
- DeepSeek  
- Mistral  
- Cohere  
- Together.ai  
- Groq  
- Perplexity  
- Gemini (Google)  
- AWS Bedrock  
- OpenRouter  
- Vertex AI *(planned)*  
- Azure OpenAI *(planned)*  

---

## Setup Using Git (Developer Mode)

1. Clone the repo:
```bash
git clone -b stable https://github.com/arvindgfx1/pixelbot.ai.git
cd pixelbot.ai
```

2. Install and run:
```bash
pnpm install
pnpm run dev
```

3. *(Optional)* Switch to `main` for beta features:
```bash
git checkout main
pnpm install
pnpm run dev
```

---

## Staying Updated

```bash
git stash
git pull
pnpm install
git stash pop
```

---

## Available Scripts

| Command               | Description                            |
|-----------------------|----------------------------------------|
| `pnpm run dev`        | Start dev server                       |
| `pnpm run build`      | Build the project                      |
| `pnpm run preview`    | Run production build locally           |
| `pnpm run start`      | Run via Wrangler for Cloudflare Pages  |
| `pnpm run deploy`     | Deploy to Cloudflare Pages             |
| `pnpm test`           | Run tests using Vitest                 |
| `pnpm run typecheck`  | Run TypeScript checks                  |
| `pnpm run lint:fix`   | Fix lint issues                        |
| `pnpm run typegen`    | Generate Wrangler TypeScript types     |

---

## Roadmap

See upcoming plans and ideas: [https://roadmap.sh/r/ottodev-roadmap-2ovzo](https://roadmap.sh/r/ottodev-roadmap-2ovzo)

---

## FAQ

- Use Claude 3 Sonnet or GPT-4 for best performance.  
- If terminal/code preview throws errors, switch models or reload.  
- Local models like Ollama may need custom base URL.  
- Docker provides isolated environment for advanced use.

---

## License

This project is MIT licensed.

**Note**: Although `pixelbot.ai` uses open-source code, the WebContainers API from Stackblitz **requires a commercial license** if used for for-profit purposes.  
Learn more here: [https://webcontainers.io/enterprise](https://webcontainers.io/enterprise)
