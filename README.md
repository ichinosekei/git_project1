# Анализ алгоритмов сортировки

## Введение
В данном документе представлен анализ амортизационной сложности пяти алгоритмов сортировки: сортировка слиянием (Merge Sort), быстрая сортировка (Quick Sort), сортировка пузырьком (Bubble Sort), поразрядная сортировка (Radix Sort), сортировка подсчетом (Counting Sort), и пирамидальная сортировка (Heap Sort). Основное внимание уделено временной и пространственной сложности каждого алгоритма.

## Алгоритмы сортировки

### Merge Sort (Сортировка слиянием)
- **Временная сложность**: `O(n log n)` во всех случаях.
- **Пространственная сложность**: `O(n)` дополнительной памяти для массива временных значений.
- **Описание**: Сортировка слиянием разбивает массив на две части, сортирует каждую из них, а затем сливает в одну отсортированную последовательность. Это стабильная сортировка, поддерживающая порядок равных элементов.

### Quick Sort (Быстрая сортировка)
- **Временная сложность**: В среднем `O(n log n)` и `O(n^2)` в худшем случае.
- **Пространственная сложность**: `O(log n)` из-за стека вызовов рекурсии.
- **Описание**: Быстрая сортировка работает по принципу разделяй и властвуй, выбирая опорный элемент и перераспределяя остальные элементы в массиве.

### Bubble Sort (Сортировка пузырьком)
- **Временная сложность**: `O(n^2)` в среднем и в худшем случае.
- **Пространственная сложность**: `O(1)`, так как сортировка выполняется на месте.
- **Описание**: Сортировка пузырьком многократно проходит через список, сравнивая и меняя местами соседние элементы, если они находятся в неправильном порядке.

### Radix Sort (Поразрядная сортировка)
- **Временная сложность**: `O(nk)`, где `k` — максимальная длина числа.
- **Пространственная сложность**: `O(n + k)`, требует дополнительного пространства для бакетов.
- **Описание**: Поразрядная сортировка обрабатывает каждую цифру числа от младшего к старшему разряду, используя стабильную сортировку для каждого прохода.

### Counting Sort (Сортировка подсчетом)
- **Временная сложность**: `O(n + k)`, где `k` — разница между максимальным и минимальным значением.
- **Пространственная сложность**: `O(k)` для хранения счетчиков.
- **Описание**: Сортировка подсчетом считает количество элементов для каждого ключа, затем использует эту информацию для размещения элементов непосредственно в их конечное место.

### Heap Sort (Пирамидальная сортировка)
- **Временная сложность**: `O(n log n)` в среднем и в худшем случае.
- **Пространственная сложность**: `O(1)`, так как сортировка на месте.
- **Описание**: Пирамидальная сортировка создает двоичную кучу из элементов массива, затем извлекает наибольшие элементы из кучи и размещает их в конец неотсортированной части массива.

## Заключение
Представленный анализ демонстрирует, что разные алгоритмы сортировки имеют различную эффективность в зависимости от размера данных и их начального расположения. При выборе алгоритма сортировки необходимо учитывать как временную, так и пространственную сложность, а также другие практические соображения, такие как стабильность и предполагаемая универсальность использования.
