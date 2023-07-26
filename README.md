# toDoListApp

# Backend Setup command step by step

yarn init
yarn add typescript -g

## tsconfig.json

`{
  "compilerOptions": {
    "target": "es6",
    "module": "commonjs",
    "outDir": "dist/js",
    "rootDir": "src",
    "strict": true,
    "esModuleInterop": true,
    "forceConsistentCasingInFileNames": true
  },
  "include": ["src/**/*"],
  "exclude": ["src/types/*.ts", "node_modules", ".vscode"]
}`

yarn add express cors mongoose
yarn add -D @types/node @types/express @types/mongoose @types/cors
yarn add -D concurrently nodemon

## nodemon.json

`{
    "env": {
        "MONGO_USER": "your-username",
        "MONGO_PASSWORD": "your-password",
        "MONGO_DB": "your-db-name"
    }
}`

# Frontend Setup command step by step

npx create-react-app frontend --template typescript
yarn add axios
npm install -D tailwindcss
npx tailwindcss init

## add following tailwind directives to your global.css/index.css file

@tailwind base;
@tailwind components;
@tailwind utilities;
