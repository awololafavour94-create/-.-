from statistics import median, multimode

# Function 1: Sum of numbers
def sum_numbers(numbers):
    return sum(numbers)


# Function 2: Average (Mean)
def calculate_mean(numbers):
    if len(numbers) == 0:
        return 0
    return sum(numbers) / len(numbers)


# Function 3: Median and Mode
def calculate_median_mode(numbers):
    if len(numbers) == 0:
        return None, None

    med = median(numbers)
    mod = multimode(numbers)

    return med, mod


# Main Program
numbers = [10, 20, 20, 30, 40, 50]

print("Numbers:", numbers)
print("Sum:", sum_numbers(numbers))
print("Mean:", calculate_mean(numbers))

median_value, mode_value = calculate_median_mode(numbers)

print("Median:", median_value)
print("Mode:", mode_value)




Numbers: [10, 20, 20, 30, 40, 50]
Sum: 170
Mean: 28.333333333333332
Median: 25.0
Mode: [20]

[Program finished]


















