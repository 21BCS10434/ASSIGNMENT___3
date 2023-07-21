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
