# Functional Tools

<!--
[![Build Status](https://dev.azure.com/thenewobjective/functional-tools/_apis/build/status/Build?branchName=master)](https://dev.azure.com/thenewobjective/functional-tools/_build/latest?definitionId=11&branchName=master)
-->

## Table of Contents

## Introduction

This library provides a number of utility decorators to enable the use of
features commonly found in functional languages for use with classes.

## Library Installation

## Usage

## Memoization

```ts
class Fib {
    @memo
    calcMemo(n: number): number {
        return n < 2 ? n : this.calcMemo(n - 1) + this.calcMemo(n - 2);
    }
    calc(n: number): number {
        return n < 2 ? n : this.calc(n - 1) + this.calc(n - 2);
    }
}

fib.calc(30) // 832040; 9ms
fib.calcMemo(30) // 832040; less than 1ms
```

## Currying

## Partial Application

## Fixed-Point

## Memoized Fixed-Point
