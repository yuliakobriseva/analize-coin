# analize-coin
def analyze_coin_growth(prices):
    growth = 0
    for i in range(1, len(prices)):
        if prices[i] > prices[i-1]:
            growth += 1
    return growth

# Пример использования функции
prices = [100, 110, 120, 130, 125, 140, 150]
growth_count = analyze_coin_growth(prices)
print(f"Количество дней с ростом цены: {growth_count}")
