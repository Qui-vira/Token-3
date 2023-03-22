# Token-3

This is a Solidity smart contract that defines an ``ERC20`` token named "OphirToken" with the symbol "OPT". It inherits from two other contracts, ``ERC20`` and ``Ownable.``

``ERC20`` is a standard interface for fungible tokens on the Ethereum blockchain. The Ownable contract is provided by the OpenZeppelin library and provides a basic access control mechanism, where the owner of the contract has certain privileges that other users do not.

The constructor function initializes the token with its ``name`` and ``symbol``, and does not take any arguments. The token is created with an initial supply of 0, since there is no ``_mint()`` function call inside the constructor.

The ``mint()`` function is a public function that allows the owner of the contract to mint new tokens to a specified address. It takes two arguments: ``to,`` which is the address that the tokens will be minted to, and amount, which is the amount of tokens ``to`` mint. The function calls the internal ``_mint()`` function inherited from ``ERC20``, which mints the specified amount of ``tokens`` to the specified address.

Note that this contract relies on external code from the OpenZeppelin library, which is imported via the ``import`` statements at the beginning of the file. The ``SPDX-License-Identifier`` comment is a standard license identifier used in Solidity contracts to indicate the license under which the code is distributed. In this case, it is the MIT license.



