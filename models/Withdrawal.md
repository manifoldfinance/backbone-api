# Withdrawal

## Properties

| Name                         | Type                        | Description                                                                                | Notes                       |
| ---------------------------- | --------------------------- | ------------------------------------------------------------------------------------------ | --------------------------- |
| **beneficiary**              | [**String**](string.md)     | The address of the recipient who will unlock funds on the remote chain. Hex-encoded.       | [optional][default to null] |
| **merkleUnderscoreproof**    | [**String**](string.md)     | The Merkle proof required to unlock funds on the MEV.                                      | [optional][default to null] |
| **merkleUnderscoreleaf**     | [**String**](string.md)     | The Merkle leaf hash of the withdrawal.                                                    | [optional][default to null] |
| **assetUnderscoreid**        | [**String**](string.md)     | The ID of the cleared asset to be withdrawn.                                               | [optional][default to null] |
| **burnUnderscoreid**         | [**String**](string.md)     | The ID of the underlying burn used to initiate this withdrawal.                            | [optional][default to null] |
| **quantity**                 | [**String**](string.md)     | The amount of the cleared asset to withdraw, as represented in the asset&#39;s base units. | [optional][default to null] |
| **initiatedUnderscoreblock** | [**BigDecimal**](number.md) | The block number when this withdrawal was initiated.                                       | [optional][default to null] |
| **owner**                    | [**String**](string.md)     | The address whose funds are being withdrawn.                                               | [optional][default to null] |

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
