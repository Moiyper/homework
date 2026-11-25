# homework
## Задание 1
```
my_dict = {1.12: 'aa', 67.9: 45, 3.11: 'ccc', 7.9: ' dd ', 9.2: ' ee ', 
           7.1: ' ff ', 0.12: ' qq ', 1.91: 'aa', 10.12: [1, 2, 3], 99.0: {9, 0, 1}}

print(min(my_dict) + max(my_dict))
```
## Задание 2
```
morse = {
    'A': '.-', 'B': '-...', 'C': '-.-.', 'D': '-..', 'E': '.', 'F': '..-.',
    'G': '--.', 'H': '....', 'I': '..', 'J': '.---', 'K': '-.-', 'L': '.-..',
    'M': '--', 'N': '-.', 'O': '---', 'P': '.--.', 'Q': '--.-', 'R': '.-.',
    'S': '...', 'T': '-', 'U': '..-', 'V': '...-', 'W': '.--', 'X': '-..-',
    'Y': '-.--', 'Z': '--..', '0': '-----', '1': '.----', '2': '..---',
    '3': '...--', '4': '....-', '5': '.....', '6': '-....', '7': '--...',
    '8': '---..', '9': '----.'
}

text = input().upper()
result = []

for char in text:
    if char in morse:
        result.append(morse[char])

print(' '.join(result))
```
## Задание 3
```
text = 'footballcyberpunkextraterritorialityconversationalistblockophthalmoscopicinterdependencemamauserfff'
char_counts = {}

for char in text:
    char_counts[char] = char_counts.get(char, 0) + 1

print(char_counts)
```
## Задание 4
```
text = input().lower()

for p in '.,!?:;-':
    text = text.replace(p, '')

words = text.split()
word_counts = {}
for word in words:
    word_counts[word] = word_counts.get(word, 0) + 1

min_count = min(word_counts.values())
result = min([w for w, count in word_counts.items() if count == min_count])
print(result)
```
