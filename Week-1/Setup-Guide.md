# Local setup
Start with the [OweBro application repository](https://github.com/vipul-LLM/Owebro), not this learning repository.

Install Git, Node.js (a supported version compatible with the project's package.json), VS Code and optionally Postman. Check `git --version`, `node -v` and `npm -v`.

```bash
git clone https://github.com/vipul-LLM/Owebro.git
cd Owebro
git switch -c wids/your-name
```

If you do not have write access, fork OweBro first, clone your fork instead, and use the original repository as upstream.

Open two terminals at the repository root. In the first:
```bash
cd Frontend
npm install
npm run
npm run dev
```
In the second:
```bash
cd backend
npm install
npm run
```
Inspect the backend package.json scripts and run the appropriate development/start script (for example npm run dev if present). Use the frontend URL printed in the terminal. Check the backend terminal for its port.

## Environment configuration
Inspect the source for environment variable names and request a development configuration from the mentor. Use a separate test database and your own development credentials. Do not commit .env files, database credentials, JWT secrets or real user data. Confirm .gitignore covers local secret files. Never reuse production credentials. If an environment variable is missing, document its name without its value.

## Debugging setup
If a command fails, check the current directory and package.json first. Read the first meaningful error, inspect browser Console and Network tabs, check server logs and test requests with Postman. Record what you tried and what happened. Do not blindly force dependency upgrades. If blocked, share sanitized logs and reproduction steps with the mentor.
