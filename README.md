# Devil Calculator 🤖🧮

A command-line calculator powered by **Google's Gemini 2.0 Flash model** using Python and `openai-agents`. This tool-driven AI agent solves arithmetic expressions using your custom logic — making it perfect for controlled, logic-specific tasks like calculators or business rules.

---

## 🛠 Technologies Used

- Python  
- Gemini 2.0 Flash (Generative Language API)  
- [`openai-agents`](https://github.com/openai/openai-agents) – to register tools and run agent workflows  
- `dotenv` – to manage API keys securely  
- `uv` – modern Python package manager for fast virtual environments

---

## 🚀 How It Works

1. Loads the Gemini API key from a `.env` file.  
2. Initializes the Gemini model using `AsyncOpenAI`.  
3. Registers multiple math functions using `@function_tool`.  
4. Sets strict agent instructions to **only use your tools**, not do math itself.  
5. Listens to user input in a loop and prints results using tool logic.

This approach ensures 100% predictable output based on your custom logic.

---

## 📦 Installation & Setup

```bash
# Clone the repository
git clone https://github.com/DanishHaji/The-Devil-Calculator-Assignment.git
cd devil_calculator

# Create and activate virtual environment using uv
uv venv
.venv\Scripts\activate         # Windows
# or
source .venv/bin/activate      # macOS/Linux

# Install dependencies
uv pip install openai-agents python-dotenv

Then create a .env file in the root:

GEMINI_API_KEY=your_actual_gemini_api_key_here
```
## 🧠 Example Prompt

Enter a calculation (e.g., '5 plus 3') or 'exit' to quit: 4 plus 4
Result: 9

Enter a calculation (e.g., '5 plus 3') or 'exit' to quit: 6 divided by 3
Result: 1.0

## 🙏 Acknowledgments

Special thanks to:

- Sir **Zia Khan** – President, PIAIC & GIAIC
- Sir **Ameen Alam** – Academics & Faculty Dean, GIAIC
- GIAIC  – for supporting open-source AI learning in Pakistan
- OpenAI – for the agents framework
- Google – for Gemini 2.0 Flash

## 🌐 Connect with Me
Made by Engr. Danish
📫 If you like this project, feel free to ⭐ the repo and connect with me on [LinkedIn](#) *(www.linkedin.com/in/danish-b5b26b190)*
🔧 Developer • AI Agent Explorer • Cloud & Web Engineer