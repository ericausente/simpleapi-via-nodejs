Here are the general steps to build a simple Node.js application in Docker. 
Make sure you have a Docker installed in your test environment. 

Then, a new file should be created called "package.json" and an index.js

```
git clone https://github.com/ericausente/simpleapi-via-nodejs.git
cd simpleapi-via-nodejs
docker build -t simple-api-app .
sudo docker run -dp 8001:3000 simple-api-app
```

The Node.js application should now be running in a Docker container and accessible via http://localhost:8000 in your web browser.

Access with the following endpoints: 

# http://10.201.10.147:8001/ 
## Output: Hello, you are visiting the / from Node.js in Docker!

# http://10.201.10.147:8001/coffee
## Output: Hello, you are visiting the /coffee from Node.js in Docker!

# http://10.201.10.147:8001/tea
## Hello, you are visiting the /tea from Node.js in Docker!
