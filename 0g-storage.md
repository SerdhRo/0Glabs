# Setting up the Storage Node

## Step 1: Install Dependencies

The dependencies are the same as for the validator node. Ensure Go is installed and set up properly.

Guide RozaS [here](https://github.com/SerdhRo/0Glabs/blob/main/0g-validator.md)

## Step 2: Install the Storage Node

Clone the repository and install the binary:

```
git clone https://github.com/0gProject/0g-storage.git
cd 0g-storage
make install
```

## Step 3: Initialize the Storage Node

Initialize the storage node:

```
0g-storage init <your_storage_node_name> --chain-id=0g
```
## Step 4: Configure the Storage Node

Update the configuration files as needed.

For example, update config.toml:

```
sed -i 's/seeds = ""/seeds = "<seeds>"/g' ~/.0g-storage/config/config.toml
```
## Step 5: Start the Storage Node

Start the node:

```
0g-storage start
```
