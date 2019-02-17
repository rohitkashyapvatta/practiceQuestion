# practiceQuestion
This includes solutions of random Array related problems.
Problem Statement: Rotate an Array with a number of rotations
Solution: 
 public static void solution(int[] inputNumbers, int rotate) {
        int[] movingNumbers = new int[inputNumbers.length];
        int count = 0;

        for (int i = inputNumbers.length - rotate; i <= inputNumbers.length - 1; i++) {
            movingNumbers[count] = inputNumbers[i];
            count++;
        }

        for (int j = 0; j < inputNumbers.length - rotate; j++) {
            movingNumbers[j + rotate] = inputNumbers[j];
        }

        for (int z = 0; z <= movingNumbers.length - 1; z++) {
            System.out.println(movingNumbers[z]);
        }
    }
