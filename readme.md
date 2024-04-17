Evergreen FastFarmer for Gigahorse
=====

A fork of FastFarmer supporting Gigahorse versions <= 3.0. </br>
For Information on FastFarmer visit the Github at https://github.com/GalactechsLLC/dg_fast_farmer </br>
For Information on Gigahorse visit the Github at https://github.com/madMAx43v3r/chia-gigahorse

Running
--------

To generate the farmer config:
```
ff_giga init 
```

To use a separate Fullnode for RPC calls during setup:
```
ff_giga init -f FULLNODE_HOST -p FULLNODE_PORT -r FULLNODE_RPC_HOST -o FULLNODE_RPC_PORT
```

For Wallets with lots of transactions, the init call runs much faster when targeting a PlotNFTs launcher_id with -l:
```
ff_giga init -l LAUNCHER_ID
```

To run the Farmer with TUI Interface(Default):
```
ff_giga
```

To run the Farmer in CLI mode:
```
ff_giga run
```

To Update the PlotNFTs in the Config:
```
ff_giga update-pool-info 
```

To Migrate a PlotNFT in the config:
```
ff_giga join-pool --pool-url <POOL_URL> --launcher-id <LAUNCHER_ID> --fee <FEE>
```

> [!TIP]
> To Print all available commands ```ff_giga --help``` <br>
> To Print Command Help ```ff_giga <COMMAND> --help```