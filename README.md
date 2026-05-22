# MinLimit.sol
MinLimit.sol
pragma solidity ^0.8.20;
contract MinLimit {
    uint public value;

    function set(uint x) public {
        require(x >= 1, "Too small");
        value = x;
    }
}
