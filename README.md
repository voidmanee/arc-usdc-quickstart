# Arc USDC Payments: Quickstart

Accept USDC on Arc testnet in a React app with viem.

## 1. Install
```bash
npm install viem wagmi
```

## 2. Configure
Arc testnet RPC: `https://rpc.testnet.arc.network`, chain id `5042002`. Put any API keys in `.env.local`.

## 3. Send a payment
```ts
await writeContract({ address: USDC, abi: erc20Abi, functionName: 'transfer', args: [RECIPIENT, parseUnits(amount, 6)] })
```

## 4. Verify
Wait for the receipt and link the transaction on the Arc explorer.

More guides in `guides/`.

