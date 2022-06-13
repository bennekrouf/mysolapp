# Base program for Solana using Anchor (kind of smart contracts framework for Solana)

Install Rust, Solana and Anchor

```
    anchor build
```

Generate a key pair

````
    solana-keygen new -o target/deploy/mysolanaapp-keypair.json
```

Link the key pair to the program

````
    solana address -k target/deploy/mysolanaapp-keypair.json
```

Update lib.rs and Anchor.toml with the generated program ID.

Run the tests:

```
    anchor test
````


Before deploying, start a local solana instance that keeps running

````
    solana-test-validator
```

Run the deployment

````
    anchor deploy
```



