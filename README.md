# ERC20-token-fixed-supply
Sample fixed supply token contract on ERC20 standard.
## Methods
### 1. function totalSupply
Returns the outstanding supply of all tokens.

    function totalSupply() constant returns (uint256)
### 2. function balanceOf
Returns the balance of the source address.

    function balanceOf(address src) constant returns (uint256)
### 3. function allowance
Returns the amount of tokens that a person can withdraw from the source address via the transferFrom function.

      function allowance(address src, address guy) constant returns (uint256)
### 4. function approve
Approves guy to withdraw tokens from msg.sender via the transferFrom function. Throws on uint overflow.

    function approve(address guy, uint256 wad) returns (bool)
### 5. function transfer
Transfers wad tokens from msg.sender to the dst address. Throws on uint overflow.

    function transfer(address dst, uint wad) returns (bool)
### 6. function transferFrom
Assumes sufficient approval set by the approve function. Transfers wad tokens from the src address to the dst address and decrements
from approvals[src][msg.sender]. Throws on uint overflow.

    function transferFrom(address src, address dst, uint wad) returns (bool)

# Imports
    import './SafeMath.sol';
    import './ERC20.sol';
# Support 
Donate Some Ether to the Developer. 
              
    Ethereum Address : 0x39886D0BFccc74D8CCb21c44534a41eC626620b3
