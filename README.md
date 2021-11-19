# Alien-worlds_Data_gather
Set of Python Jupyter Notebooks to gather NFT data from Alien Worlds game (https://alienworlds.io/) hosted in WAX blockchain.
It requires the ***Dalton-API*** library (https://pypi.org/project/daltonapi/) to get data from WAX blockchain and ***Pandas***.

# Lands Extrac and transform
This notebook gets all information regarding each Land in the game: planet, owner, mining comission, ease, luck.
So far there are just +3k lands and is not expected to grow in the near future. The last planet create has no lands. Therefore it just collect them all format and transform some features and save it to a CSV file.

# Tools extractor and transfrom
This notebook gets all information of every tool minted in the game, burned or not. It will get every pice of information available in the blockchain for each tool: owner, minting date, burned, luck, ease, and more.
The number of tools will increase constantly, rigth now is +300k. Because of this, the amount of time and memory it will take there is a need of saving the collected data while is being colected. The script will be saving to a CSV when 50k tool are gathered and adding to this file every time it reaches that count.
