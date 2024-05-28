n, f = list(map(int, input().split()))
matriz, pilha = [], [(0,0)]

for _ in range(n):
    matriz.append(list(map(int, input())))

while pilha:
    x, y = pilha.pop()
    if matriz[x][y] != '*' and f >= matriz[x][y]:
        matriz[x][y] = '*'
        if x < n - 1:
            pilha.append((x + 1, y))
        if y < n - 1:
            pilha.append((x, y + 1))
        if x > 0:
            pilha.append((x - 1, y))
        if y > 0:
            pilha.append((x, y - 1))
            
for i in matriz:
    print(''.join([str(y) for y in i]))
