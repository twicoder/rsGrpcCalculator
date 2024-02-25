# Readme

- This is simple gRPC demo writen in Rust


# Operations
```

grpcurl -plaintext -d '{\"a\":111,\"b\":222}' '[::1]:50051' calculator.Calculator.Add

grpcurl -plaintext -d '{\"a\":200,\"b\":100}' '[::1]:50051' calculator.Calculator.Divide

grpcurl -emit-defaults -plaintext '[::1]:50051' calculator.Admin.GetRequestCount

grpcurl -plaintext '[::1]:50051' list

grpcurl -H "Authorization: Bearer some-secret-token" -emit-defaults -plaintext '[::1]:50051' calculator.Admin.GetRequestCount

```






