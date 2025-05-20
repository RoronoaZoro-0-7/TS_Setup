command used to set this ts folder in backend are 

npm i bcryptjs cookie-parser cors dotenv express ioredis jsonwebtoken mongoose
npm i -D ts-node-dev typescript @types/bcryptjs @types/cookie-parser @types/cors @types/express @types/jsonwebtoken @types/node

npx tsc --init

change tsconfig.json to this : 

{
  "compilerOptions": {
    "target": "ES2020",
    "module": "ESNext",
    "moduleResolution": "Node",
    "esModuleInterop": true,
    "forceConsistentCasingInFileNames": true,
    "strict": true,
    "skipLibCheck": true
  },
  "include": ["./"]
}

npm i -D tsx

in package.json inside scripts add this line :
"dev": "tsx watch index.ts"
