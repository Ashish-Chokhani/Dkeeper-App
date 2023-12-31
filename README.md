# dkeeper

Welcome to my new dkeeper project and to the internet computer development. 

## Running the project locally

If you want to test your project locally, you can use the following commands:

```bash
# Starts the replica, running in the background
dfx start --background

# Deploys your canisters to the replica and generates your candid interface
dfx deploy
```

Once the job completes, the application will be available at `http://localhost:8080?canisterId={asset_canister_id}`.

Additionally, if anyone is making frontend changes, you can start a development server with

```bash
npm start
```

Which will start a server at `http://localhost:8080`, proxying API requests to the replica at port 8000.
