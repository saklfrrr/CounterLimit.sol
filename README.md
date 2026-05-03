# CounterLimit.sol
CounterLimit.sol
pragma solidity ^0.8.20;
contract CounterLimit {
    uint public count;

    function inc() public {
        require(count < 100, "Max reached");
        count++;
    }
}
