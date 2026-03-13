
# Insertion Sort Program

n = int(raw_input("Enter number of elements: "))
a = []

for i in range(n):
    x = int(raw_input("Enter element: "))
    a.append(x)

for i in range(1, n):
    key = a[i]
    j = i - 1

    while j >= 0 and a[j] > key:
        a[j + 1] = a[j]
        j = j - 1

    a[j + 1] = key

print "Sorted elements are:"
for i in range(n):
    print a[i]

OUTPUT 


Enter number of elements: 5
Enter element: 50
Enter element: 20
Enter element: 40
Enter element: 10
Enter element: 30

Sorted elements are:
10
20
30
40
50
