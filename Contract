// SPDX-License-Identifier: MIT
pragma solidity ^0.8.0;

import "@openzeppelin/contracts/token/ERC20/IERC20.sol";
import "./interfaces/IUniswapV2Pair.sol";

contract FlashArbitrage {
    // Uniswap call back function
    function uniswapV2Call(address sender, uint amount0, uint amount1, bytes calldata data) external {
        // 1. Check if the call came from a real Uniswap Pair
        // 2. Logic to Swap on Sushiswap
        // 3. Logic to check Profit
        // 4. Repay Uniswap
    }

    function startArbitrage(address pairAddress, uint amountToBorrow) external {
        // Trigger Flash Swap
        IUniswapV2Pair(pairAddress).swap(amountToBorrow, 0, address(this), new bytes(1));
    }
}
