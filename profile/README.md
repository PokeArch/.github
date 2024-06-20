# PokéArch
PokéArch is a Godot Engine Based game built for the Archway ecosystem using ArchID and Andromeda Embeddables. PokéArch offers a dynamic and immersive experience with multiple environments, a seamless UI, and strategic gameplay. The game has the old-school Pokémon theme along with nostalgic sound effects which make the experience even more immersive. 

# How to Play

## Setup

1. Go to the [PokeArch Website](https://pokearch.netlify.app/)
2. Connect using Keplr Wallet
3. Register/Login with your Existing ArchID
4. Follow along and Accept the Keplr Popups and Get a [Bulbasaur](https://embeddables.testnet.andromedaprotocol.io/constantine-3/PokeArch/embeddables-auction-1/cw721/0) for free

## Battles

1. Move around the grassy areas to encounter Pokemons
2. Battle with Pokemons and try to catch them once their Health is less than 40
3. Get a Pokemon NFT upon successfully catching the Pokemon.

## Friendly Battle

1. Open the Inventory by Pressing I
2. Select the 'Multiplayer Menu'
3. Enter your friend's ArchID
4. Fight with their default Pokemon

## Berries

1. Go near the trees where you see the berries.
2. Press B to collect.
3. Open the Inventory.
4. Feed the berries to your Pokemons.

# Technologies Used

- **Godot Engine** - Used for creating the game.
- **JavaScript** - Used for integrating the game with Archway.
- **Archway Testnet** - Blockchain on which the smart contracts are deployed.
- **CosmWasm(Rust)** - Used for [smart contracts](https://github.com/PokeArch/contracts/blob/main/contracts/pokearch/src/contract.rs) development.
- **Webpack** - For compiling the files.
- **ArchID** - Used for User Identification.
- **Andromeda Protocol** - NFT Auction [Embeddable](https://embeddables.testnet.andromedaprotocol.io/constantine-3/PokeArch)
- **Pinata** - Used for storing NFT metadata

# Working

## User Identification (ArchID)
PokeArch provides an easy and simple way to register archIDs to the new users. Users also may use their existing archIDs to play the game. The player details are mapped with their archIDs. 

1 ArchID = 1 PokeArch Account

This allows players to have multiple accounts using one wallet.

ArchIDs also allow players to challenge their friends and battle with the Pokemon set as the default for their ArchID.

## Catching Pokemons(Archway NFTs)
Everytime a Pokemon is caught, a new NFT is minted for the player. The player can directly trade these NFTs with anyone.

These NFTs contain the pokemon details such as Type, Special Attack, etc.

## Gas Fees Grants (cw-fee module)
Players can also get grants for the gas fees payments once they're added to the allowed-list. This makes the experience more user friendly.

# Challenges that we faced

- Godot doesn't have good support for the blockchain integrations, we had to do alot of googling in order to get everything working.
- Error messages are not well formatted. This consumed alot of our time.

# What's Next for PokeArch
- Built-in Pokemon NFTs Auctions
- Currently, there are only a few pokemons. So, we need to add some more.
- Refining the maps.
- Get a feedback from the Archway Team to deploy on the Mainnet

# Deployed Contracts
All the contracts are deployed on the ```constantine-3``` chain.
```
POKEARCH_CONTRACT = archway1mg4wqfx7546d46ddss8tajkhscwc5dhrud494ct99zpusp9qqunssrgezp
NFT_CONTRACT = archway1mg4wqfx7546d46ddss8tajkhscwc5dhrud494ct99zpusp9qqunssrgezp
ADO_APP_CONTRACT = archway1uqq3z9fhu7vhtfm9wzns8m79msqtq6qxc3ckdutln9u269u8yz3qgj5hpk
ADO_APP_AUCTION = archway1vdjm9ehcce38eqsvfrwy3dglxd03mxx4gqgaea5m7and3qjd758qh5qtpg
```