# START PRJECT WITH TYPESCRIPT

[
npm init --yes
npm install express dotenv
npm i -D typescript @types/express @types/node
npx tsc --init
]

## tsconfig.json

target: es2016
module: commonjs
strict: true
esModuleInterop: true
skipLibCheck: true
forceConsistentCasingInFileNames: true


{
  "compilerOptions": {
    "outDir": "./dist"
  }
}

[npm install -D concurrently nodemon]

## package.json

    {
    "scripts": {
        "build": "npx tsc",
        "start": "node dist/index.js",
        "dev": "concurrently \"npx tsc --watch\" \"nodemon -q dist/index.js\""
        }
    }


## finally
yarn install yarn run dev
