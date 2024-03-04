- 👋 Hi, I’m @ALVESTX4
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
ALVESTX4/ALVESTX4 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
def is_prime(num):
    if num < 2:
        return False
    for i in range(2, int(num ** 0.5) + 1):
        if num % i == 0:
            return False
    return True

def find_primes(start, end):
    primes = [num for num in range(start, end + 1) if is_prime(num)]
    return primes

if __name__ == "__main__":
    start_range = int(input("Digite o início do intervalo: "))
    end_range = int(input("Digite o final do intervalo: "))

    prime_numbers = find_primes(start_range, end_range)

    print(f"Números primos no intervalo de {start_range} a {end_range}:")
    print(prime_numbers)

