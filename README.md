# Type Instability Bug in Julia

This repository demonstrates a common performance issue in Julia: type instability. The `my_function` in `bug.jl` exhibits this problem because it can return both `Int64` and `Float64` depending on input.  This causes the JIT compiler to generate slower code.

The solution in `bugSolution.jl` showcases how to improve the type stability of the function.