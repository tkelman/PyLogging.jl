# PyLogging.jl

## Overview

This is a Julia wrapper for Python logging package.

## Example

```{julia}
using PyLogging

PyLogging.basicConfig(
	level=PyLogging.INFO,
	format="%(asctime)s - %(name)s - %(message)s"
)

root = getLogger()
loggerA = getLogger("a")

@debug loggerA "debug"
@info loggerA "info"
```
