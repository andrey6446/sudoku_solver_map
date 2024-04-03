# sudoku_solver_map

input - "1-58-2----9--764-52--4--819-19--73-6762-83-9-----61-5---76---3-43--2-5-16--3-89---" - сразу лучше преобразовать в двумерный массив 9 х 9

output - "145892673893176425276435819519247386762583194384961752957614238438729561621358947"

functions: 

1. solve(board) - главная функция возвращает output, если findEmpty(board) === null то судоку решен

2. findEmpty(board) - функция поиска пустых ячеек на доске (то есть "-", возвращает массив [r (строка) ,c (колонка) ], если пустых ячеек нет - возвращает null

3. validate(currentNum, currentPosition, board) - функция проверки доски на валидность после подстановки некого значения, функция возвращает true, если в строке, столбце и боксе 3х3 нет нашего currentNum

4. stringTo2DArray
