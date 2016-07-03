# Split.jl

[![Build Status](https://travis-ci.org/maarek/Split.jl.svg?branch=master)](https://travis-ci.org/maarek/Split.jl)

Package for sampling Julia DataFrames into a uniform random sample by percentage and seed and loading them into a Training Set and a Test Set.

## Installation
```julia
Pkg.add("Split")
```

## Usage

Split.jl provides a high-level method '**sample**' for returning a uniform random sample of a DataFrame, that contains percent of the total elements, without replacement, using a random seed.
```julia
(train, test) = Split.sample(df::AbstractDataFrame, fraction::Real, seed::Integer)
```
