Generators in Python are used to produce values one at a time, pausing execution with `yield` and resuming later, which makes them ideal for efficient, memory‑friendly iteration over large or infinite sequences.

# generator_file_line
This project demonstrates how to use Python's `yield` keyword to read a file line by line efficiently.  
Instead of loading the entire file into memory, the generator delivers one line at a time and pauses until the next request.

## File
- `generator_file_line.py`: contains the generator function and usage examples.

## Example
```python
def read_file(file_name):
    with open(file_name, "r", encoding="utf-8") as f:
        for line in f:
            yield line.strip()

gen = read_file("dados.txt")

print(next(gen))  # first line
print(next(gen))  # second line

