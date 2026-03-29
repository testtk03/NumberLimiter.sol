# NumberLimiter.sol
Base - Smart Contract Deployed by Remix NumberLimiter.sol
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.20;

contract NumberLimiter {
    uint public number;

    function setNumber(uint _number) public {
        require(_number <= 100, "Number too large");
        number = _number;
    }
}
