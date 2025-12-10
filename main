def read_file(file_name):
    with open(file_name, "r", encoding="utf-8") as f:
        for line in f:
            yield line.strip()

gen = read_file("dados.txt")

print(next(gen))
print(next(gen))
print(next(gen))
print(next(gen))
