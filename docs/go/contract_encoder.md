---
slug: /contract_encoder
title: Contract Encoder
hide_title: true
displayed_sidebar: go
---

## Contract Encoder

This interface is currently supported by all contract encoder classes and provides a generic method to encode write function calls\.

```go
type ContractEncoder struct {}
```

### func \(\*ContractEncoder\) [Encode](https://github.com/thirdweb-dev/go-sdk/blob/main/thirdweb/contract_encoder.go#L56)

```go
func (encoder *ContractEncoder) Encode(method string, args ...interface{}) (*types.Transaction, error)
```

Get the unsigned transaction data for any contract call on a contract\.

method: the name of the contract function to encode transaction data for

args: the arguments to pass to the contract function\.

returns: the encoded transaction data for the transaction\.

#### Example

```
toAddress := "0x..."
amount := 1

// Now you can get the transaction data for the contract call.
tx, err := contract.Encoder.Encode("transfer", toAddress, amount)
```

fmt\.Println\(tx\.Data\(\)\) // Now you can access all transaction data, like the following fields fmt\.Println\(tx\.Nonce\(\)\) fmt\.Println\(tx\.Value\(\)\)