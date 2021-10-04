# UnsafeMath

Lib for avoiding checks on solidity 8 and saving gas

```
// SPDX-License-Identifier: MIT

pragma solidity ^0.8.0;


library UnsafeMath {

    function unsafeAdd(uint256 a, uint256 b) internal pure returns (uint256) {
        unchecked {
            return a + b;
        }
    }

    function unsafeSub(uint256 a, uint256 b) internal pure returns (uint256) {
        unchecked {
            return a - b;
        }
    }

    function unsafeMul(uint256 a, uint256 b) internal pure returns (uint256) {
        unchecked {
            return a * b;
        }
    }

}
```
