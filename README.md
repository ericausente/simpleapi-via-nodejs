Here are the general steps to build a simple Node.js application in Docker. 
Make sure you have a Docker installed. 

Then, a new file should be created called "package.json" and an index.js

```
git clone https://github.com/ericausente/simpleapi-via-nodejs.git
cd simpleapi-via-nodejs
docker build -t simple-api-app .
docker run -dp 8000:3000 your-app-name
```

The Node.js application should now be running in a Docker container and accessible via http://localhost:8000 in your web browser.
