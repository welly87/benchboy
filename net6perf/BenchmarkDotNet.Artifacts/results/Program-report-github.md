``` ini

BenchmarkDotNet=v0.13.1, OS=amzn 2022
Unknown processor
.NET SDK=6.0.400
  [Host]     : .NET 6.0.8 (6.0.822.36306), Arm64 RyuJIT
  Job-ENSLBL : .NET 6.0.8 (6.0.822.36306), Arm64 RyuJIT

Runtime=.NET 6.0  Toolchain=net6.0  

```
| Method |     Mean |    Error |   StdDev | Allocated |
|------- |---------:|---------:|---------:|----------:|
| Format | 12.56 ns | 0.002 ns | 0.002 ns |         - |
