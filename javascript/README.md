# Build requirements

* Node.js
* Red Hat Datagrid 8 Server

# Build instructions

    npm install

# Run instructions 

1. Create an admin user `./bin/cli.sh user create admin -p password`
  
2. Start the server calling `./bin/server.sh` (Linux, OS X, Unix) or 
  `bin/server.bat` (Windows).
3. Create a cache named `my-cache` using the [Data Grid Console](http://localhost:11222/)
  ```json
  "distributed-cache": {
    "mode": "SYNC",
    "encoding": {
    "media-type": "text/plain"
    },
    "statistics": true
  }
```
4. Execute: `node index.js`

5. Check with the Data Grid Console [the my-cache cache detail](http://localhost:11222/console/my-cache)
