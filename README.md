# Eme
addMatrices(matrixA, matrixB, sumMatrix, N);
 System.out.println("The sum of the matrices is:");
 displayMatrix(sumMatrix);
 }
 public static void enterMatrixElements(int[][] matrix, Scanner scanner) {
 for (int i = 0; i < matrix.length; i++) {
 for (int j = 0; j < matrix[0].length; j++) {
 System.out.print("Enter element [" + i + "][" + j + "]: ");
 matrix[i][j] = scanner.nextInt();
 }
 }
 }
 public static void addMatrices(int[][] matrixA, int[][] matrixB, int[][] sumMatrix, int N) {
 for (int i = 0; i < N; i++) {
 for (int j = 0; j < N; j++) {
 sumMatrix[i][j] = matrixA[i][j] + matrixB[i][j];
 }
 }
 }
 public static void displayMatrix(int[][] matrix) {
 for (int[] row : matrix) {
 for (int element : row) {
 System.out.print(element + " ");
 }
 System.out.println();
 }
 }
}
