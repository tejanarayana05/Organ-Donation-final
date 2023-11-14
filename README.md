## Prerequisites

You would need these software installed on your machine to run the project.
### node.js

  1. Delete the existing Node from control panel
  2.Visit the NodeJS web page at https://nodejs.org/en/
  3. Download and install the LTS version.
  4. Download the installer and run it. This will install both NodeJS and NPM (Node Package Manager).
  

### Truffle
Open the command prompt or terminal and execute the following command.
```sh
npm install -g truffle
```

### Ganache
Visit the Ganache webpage at http://trufflesuite.com/ganache/
Download the platform binary for your OS and install it.

### Git

### Download
1. Open gitbash or terminal.
2. Clone the repo.
   ```sh
   git clone https://github.com/tejanarayana05/Organ-Donation-final
   ```
3. Traverse into the app folder.
   ```sh
   cd organ-donation-platform/app
   ```
4. Install npm dependencies.
   ```sh
   npm install
   ```

### Connect Ganache
While the npm dependencies are being installed, follow these instructions.

1. Open ganache.
2. Click on "New Workspace".
3. Give Name of project
4. Select "Add Project button" and add the truffle-config.js file located in the folder "organ-donation-platform" you just downloaded.
4. Confirm by pressing "Save Workspace" on the top-right corner.

5. Navigate to the "Contracts" tab and you should notice DonorContract is not deployed.

### Deploy Contract
Back in the gitbash or terminal window instance in which you were downloading npm dependencies, wait for it to finish up and then type in the following commands to deploy the contract.
```sh
truffle compile && truffle migrate
```

### Run the server
Now that everything is set-up, you can run the server.
1. Run the following command
   ```sh
   npm run dev
   ```
2. Open a browser and go to http://localhost:8080/