def dibagi_5(n):
    return (10**n + 6**n + 1) % 5 == 0

def membuktikan_induksi():
    print("Membuktikan dengan induksi matematika bahwa 10^n + 6^n + 1 habis dibagi oleh 5")
    print("Langkah 1: Base Case")
    for n in range(3):
        print(f"n = {n}: 10^{n} + 6^{n} + 1 = {10**n + 6**n + 1}, dibagi 5: {dibagi_5(n)}")
    print("\n Langkah 2: Langkah Induksi")
    for n in range(3,11):
        print(f"n = {n}: 10^{n} + 6^{n} + 1 = {10**n + 6**n + 1}, dibagi 5: {dibagi_5(n)}")

membuktikan_induksi()
