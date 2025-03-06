# bubble2D

#### Implementa en Java el método de ordenación de la burbuja para un array bidimensional (o matriz) de números enteros. Este método debe recibir una array bidimensional como parámetro y permitir la ordenación tanto ascendente como descendente. El tipo de ordenación (ascendente o descendente) se especificará mediante un parámetro booleano a vuestro criterio. 

## Pseudo

      function bubbleSort2D(matrix, ascending)
          if matrix is null or matrix has no elements
              return null
      
          rows = number of rows in matrix
          columns = number of columns in matrix
          totalElements = rows * columns
      
          for i = 0 to totalElements - 2
              for j = 0 to totalElements - i - 2
                  currentRow = j / columns
                  currentColumn = j % columns
                  nextRow = (j + 1) / columns
                  nextColumn = (j + 1) % columns
      
                  if ascending
                      if matrix[currentRow][currentColumn] > matrix[nextRow][nextColumn]
                          swap matrix[currentRow][currentColumn] and matrix[nextRow][nextColumn]
                      end if
                  else
                      if matrix[currentRow][currentColumn] < matrix[nextRow][nextColumn]
                          swap matrix[currentRow][currentColumn] and matrix[nextRow][nextColumn]ç
                      end if
                  end if
              end for
           end for
