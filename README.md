# Parquet .NET for Dyalog
This is a Tatin package for Dyalog APL for reading `.parquet` files as inverted tables.

This package depends on .NET (currently the .NET SDK 6.0 or higher).

## Get the package
Currently **ParquetDotNet** is only available as a Cider project while we are working out the best way to distribute the package's .NET dependencies.

1. Clone this repository
1. Open with Cider:

```
]Cider.OpenProject /path/to/ParquetDotNet/
```

## Read parquet file
The *Read* function returns a 2-element result: the data and the header.

```
(data header)←ParquetDotNet.Read'/path/to/file.parquet'
```

A sample is provided in `tests`.

## Data types
|C# type|APL type|
|  ---  |   ---  |
|String | Character vector or matrix |
|Int32  | Number |
|DateTime | Dyalog Date Number (see [`⎕DT`](http://help.dyalog.com/latest/#Language/System%20Functions/dt.htm)) |

## TO DO

- [x] Create Cider project and Tatin package
- [x] Use Parquet.NET NuGet package
- [ ] Test publishing tatin package
- [ ] Create Make function for deployment
- [ ] Make function handles Version
- [ ] Write minimum docs and tests
- [ ] Make the docs not lies
- [ ] Make the tests not lies
