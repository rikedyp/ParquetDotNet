# How to create a package in Dyalog APL

In this tutorial, I will summarise the steps necessary to set up development and deployment of a Tatin package using the Cider project manager for Dyalog APL.

## Set up your working environment
1. Install the Tatin client (already available in Dyalog from version 19.0 onwards)
1. Install the Cider project manager

## Create the Cider project

## Create the Tatin package

## Managing non-APL assets
A project may depend on non-APL files which reside outside of the workspace and APL source code.

## Example: ParquetDotNet
As an example, I will show the steps to set up development and deployment of the [rikedyp]/ParquetDotNet package.

This package depends on third party shared libraries. I have obtained these from NuGet, but include them in the package assets so that they are available to the user once they load or install the package via Tatin.

### Loading .NET libraries
When developing with **Cider**, the project's assets are relative to `ParquetDotNet.CiderConfig.HOME`.

When a user has loaded `ParquetDotNet` from **Tatin**, the project's assets are relative to `(⊃⊃⎕CLASS ⎕THIS).##.TatinVars.GetFullPath2AssetsFolder`.
