# mern-stack-example
Mern Stack code for the [Mern Tutorial](https://www.mongodb.com/languages/mern-stack-tutorial)

[![CI](https://github.com/mongodb-developer/mern-stack-example/actions/workflows/main.yaml/badge.svg)](https://github.com/mongodb-developer/mern-stack-example/actions/workflows/main.yaml)

## How To Run
Create an Atlas URI connection parameter in `mern/server/config.env` with your Atlas URI:
```
ATLAS_URI=mongodb+srv://<username>:<password>@sandbox.jadwj.mongodb.net/myFirstDatabase?retryWrites=true&w=majority
PORT=5000
```

Start server:
```
cd mern/server
npm install
npm start
```

Start Web server
```
cd mern/client
npm install
npm start
```

### Issues

#### `Error: error:0308010C:digital envelope routines::unsupported`

https://stackoverflow.com/questions/69692842/error-message-error0308010cdigital-envelope-routinesunsupported


I am using node v18

quick fix:
```
npm audit fix --force
```

### [Source](https://github.com/wgong/mern-stack-example)

## Disclaimer

Use at your own risk; not a supported MongoDB product
