# Parquet .NET for Dyalog
This is a Tatin package for Dyalog APL for reading `.parquet` files as inverted tables.

## Data types
|C# type|APL type|
|  ---  |   ---  |
|String | Character vector or matrix |
|Int32  | Number |
|DateTime | Dyalog Date Number (see [`⎕DT`](http://help.dyalog.com/latest/#Language/System%20Functions/dt.htm)) |

## Get the package
Load the package with Tatin:

## Read parquet file
A sample is provided in `tests`.

## TO DO

- [x] Create Cider project and Tatin package
- [ ] Check out NuGetConsum to get NuGet package rather than host files separately.
- [ ] Set up to handle assets appropriately for Cider dev and Tatin deploy
- [ ] Create Make function for deployment, including copying README as docs index?
- [ ] Test publishing tatin package
- [ ] Write minimum docs and tests
- [ ] Make the docs not lies
- [ ] Make the tests not lies
