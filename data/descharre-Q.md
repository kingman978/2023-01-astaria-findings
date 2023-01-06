# Summary
|ID     | Finding| Instances |
|:----: | :---           |              :----:    |  :----:         |
|1       | Use a literal instead of functions for a constant  | 1 |
| 2      | REQUIRE() OR REVERT() STATEMENTS THAT CHECK INPUT ARGUMENTS SHOULD BE AT THE TOP OF THE FUNCTION| 1 |
| 3      |Missing error messages in require statements| 1 |
| 4      |Add natspec documentation| 1 |
| 3      |Miscellaneous| 1 |

# Details
## 1 
[CollateralToken.sol#L73](https://github.com/code-423n4/2023-01-astaria/blob/main/src/CollateralToken.sol#L73)

## 2
[CollateralToken.sol#L564](https://github.com/code-423n4/2023-01-astaria/blob/main/src/CollateralToken.sol#L564)
[PublicVault.sol#L170](https://github.com/code-423n4/2023-01-astaria/blob/main/src/PublicVault.sol#L170)

This can also be done for some if statements
[CollateralToken.sol#L109-L134](https://github.com/code-423n4/2023-01-astaria/blob/main/src/CollateralToken.sol#L109-L134)
[AstariaRouter.sol#L466](https://github.com/code-423n4/2023-01-astaria/blob/main/src/AstariaRouter.sol#L466)

## 3 Missing error messages in require statements
Usage of error messages in require statements can help at monitoring and debugging. There is also an option to make these if statements with custom error messages
- [AstariaRouter.sol#L341](https://github.com/code-423n4/2023-01-astaria/blob/main/src/AstariaRouter.sol#L341)
- [AstariaRouter.sol#L347](https://github.com/code-423n4/2023-01-astaria/blob/main/src/AstariaRouter.sol#L347)
- [AstariaRouter.sol#L354](https://github.com/code-423n4/2023-01-astaria/blob/main/src/AstariaRouter.sol#L354)
- [AstariaRouter.sol#L361](https://github.com/code-423n4/2023-01-astaria/blob/main/src/AstariaRouter.sol#L361)
- [ClearingHouse.sol#L72](https://github.com/code-423n4/2023-01-astaria/blob/main/src/ClearingHouse.sol#L72)
- [ClearingHouse.sol#L199](https://github.com/code-423n4/2023-01-astaria/blob/main/src/ClearingHouse.sol#L199)
- [ClearingHouse.sol#L216](https://github.com/code-423n4/2023-01-astaria/blob/main/src/ClearingHouse.sol#L216)
- [ClearingHouse.sol#L223](https://github.com/code-423n4/2023-01-astaria/blob/main/src/ClearingHouse.sol#L223)
- [CollateralToken.sol#L266](https://github.com/code-423n4/2023-01-astaria/blob/main/src/CollateralToken.sol#L266)
- [CollateralToken.sol#L535](https://github.com/code-423n4/2023-01-astaria/blob/main/src/CollateralToken.sol#L535)
- [CollateralToken.sol#L564](https://github.com/code-423n4/2023-01-astaria/blob/main/src/CollateralToken.sol#L564)
- [LienToken.sol#L504](https://github.com/code-423n4/2023-01-astaria/blob/main/src/LienToken.sol#L504)
- [LienToken.sol#L860](https://github.com/code-423n4/2023-01-astaria/blob/main/src/LienToken.sol#L860)
- [PublicVault.sol#L241](https://github.com/code-423n4/2023-01-astaria/blob/main/src/PublicVault.sol#L241)
- [PublicVault.sol#L259](https://github.com/code-423n4/2023-01-astaria/blob/main/src/PublicVault.sol#L259)
- [PublicVault.sol#L508](https://github.com/code-423n4/2023-01-astaria/blob/main/src/PublicVault.sol#L508)
- [PublicVault.sol#L672](https://github.com/code-423n4/2023-01-astaria/blob/main/src/PublicVault.sol#L672)
- [PublicVault.sol#L680](https://github.com/code-423n4/2023-01-astaria/blob/main/src/PublicVault.sol#L680)
- [PublicVault.sol#L687](https://github.com/code-423n4/2023-01-astaria/blob/main/src/PublicVault.sol#L687)
- [Vault.sol#L65](https://github.com/code-423n4/2023-01-astaria/blob/main/src/Vault.sol#L65)
- [Vault.sol#L71](https://github.com/code-423n4/2023-01-astaria/blob/main/src/Vault.sol#L71)
- [VaultImplementation.sol#L78](https://github.com/code-423n4/2023-01-astaria/blob/main/src/VaultImplementation.sol#L78)
- [VaultImplementation.sol#L96](https://github.com/code-423n4/2023-01-astaria/blob/main/src/VaultImplementation.sol#L96)
- [VaultImplementation.sol#L105](https://github.com/code-423n4/2023-01-astaria/blob/main/src/VaultImplementation.sol#L105)
- [VaultImplementation.sol#L114](https://github.com/code-423n4/2023-01-astaria/blob/main/src/VaultImplementation.sol#L114)
- [VaultImplementation.sol#L147](https://github.com/code-423n4/2023-01-astaria/blob/main/src/VaultImplementation.sol#L147)
- [VaultImplementation.sol#L191](https://github.com/code-423n4/2023-01-astaria/blob/main/src/VaultImplementation.sol#L191)
- [VaultImplementation.sol#L211](https://github.com/code-423n4/2023-01-astaria/blob/main/src/VaultImplementation.sol#L211)
- [WithdrawProxy.sol#L138](https://github.com/code-423n4/2023-01-astaria/blob/main/src/WithdrawProxy.sol#L138)
- [WithdrawProxy.sol#L231](https://github.com/code-423n4/2023-01-astaria/blob/main/src/WithdrawProxy.sol#L231)
## Miscellaneous
### Casting to uint256 is not necessary
[AstariaRouter.sol#L531-L540](https://github.com/code-423n4/2023-01-astaria/blob/main/src/AstariaRouter.sol#L531-L540)