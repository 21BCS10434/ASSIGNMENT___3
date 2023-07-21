  // SPDX-License-Identifier: MIT
pragma solidity ^0.8.0;

contract EvenOrOdd {
    function checkEvenOrOdd(uint256 _number) external pure returns (string memory) {
        // Using require statement
        require(_number > 0, "Number must be positive");

        // Using assert statement
        assert(_number <= type(uint256).max / 2 + 1);

        // Using require statement
        require(_number % 2 == 0 || _number % 2 == 1, "Invalid number");

        if (_number % 2 == 0) {
            return "Even";
        } else {
            return "Odd";
        }
    }
}
