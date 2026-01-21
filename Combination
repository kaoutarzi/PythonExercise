"""
Computation of combinations C(n, k)
"""

from math import comb


def fact_iter(n):
    """Iterative factorial"""
    result = 1
    for i in range(2, n + 1):
        result *= i
    return result


def fact_rec(n):
    """Recursive factorial"""
    if n <= 1:
        return 1
    return n * fact_rec(n - 1)


def comb_iter(n, k):
    """Combination using iterative factorial"""
    return fact_iter(n) // (fact_iter(k) * fact_iter(n - k))


def comb_rec(n, k):
    """Combination using recursive factorial"""
    return fact_rec(n) // (fact_rec(k) * fact_rec(n - k))


def comb_math(n, k):
    """Combination using math library"""
    return comb(n, k)


# Example
if __name__ == "__main__":
    n = 5
    k = 2
    print("Iterative factorial:", comb_iter(n, k))
    print("Recursive factorial:", comb_rec(n, k))
    print("Math library:", comb_math(n, k))
