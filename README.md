## Comparison of flash loan service on Ethereum

### Results
Obtained via:
```shell
$ forge test --fork-url $NODE_URL --gas-report --optimize --optimize-runs 10
```

#### AAVE
```
╭──────────────────┬─────────────────┬───────┬────────┬────────┬─────────╮
│ AAVE contract    ┆                 ┆       ┆        ┆        ┆         │
╞══════════════════╪═════════════════╪═══════╪════════╪════════╪═════════╡
│ Deployment Cost  ┆ Deployment Size ┆       ┆        ┆        ┆         │
├╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌┼╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌┼╌╌╌╌╌╌╌┼╌╌╌╌╌╌╌╌┼╌╌╌╌╌╌╌╌┼╌╌╌╌╌╌╌╌╌┤
│ 302169           ┆ 1556            ┆       ┆        ┆        ┆         │
├╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌┼╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌┼╌╌╌╌╌╌╌┼╌╌╌╌╌╌╌╌┼╌╌╌╌╌╌╌╌┼╌╌╌╌╌╌╌╌╌┤
│ Function Name    ┆ min             ┆ avg   ┆ median ┆ max    ┆ # calls │
├╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌┼╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌┼╌╌╌╌╌╌╌┼╌╌╌╌╌╌╌╌┼╌╌╌╌╌╌╌╌┼╌╌╌╌╌╌╌╌╌┤
│ executeOperation ┆ 24509           ┆ 24719 ┆ 24509  ┆ 26609  ┆ 10      │
├╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌┼╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌┼╌╌╌╌╌╌╌┼╌╌╌╌╌╌╌╌┼╌╌╌╌╌╌╌╌┼╌╌╌╌╌╌╌╌╌┤
│ go               ┆ 69674           ┆ 82550 ┆ 69674  ┆ 198434 ┆ 10      │
╰──────────────────┴─────────────────┴───────┴────────┴────────┴─────────╯
```

### TODO
[x] AAVE
[] Balancer
[] Euler
[] Uniswap