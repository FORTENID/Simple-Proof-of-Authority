# Simple-Proof-of-Authority
A basic consensus mechanism using a simple proof-of-authority algorithm.
class Node:
    def __init__(self, address):
        self.address = address

def validate_block(block, last_block):
    # Simple proof-of-authority validation logic
    return block.proof > last_block.proof

# Example usage
node_A = Node("Node A")
node_B = Node("Node B")

# Assume there is a broadcast of blocks between nodes
new_block = get_new_block_from_network()

if validate_block(new_block, last_block):
    blockchain.append(new_block)
