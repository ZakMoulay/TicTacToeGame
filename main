import java.util.List;
import java.util.Arrays;
import java.util.ArrayList;
import java.util.Scanner;
import java.util.Random;;
public class TicTocToe {
    static ArrayList<Integer> playerPositions = new ArrayList<>();
    static ArrayList<Integer> cpuPositions = new ArrayList<>();

    public static void main(String[] args) {
        char[][] gameBoard = {{' ', '|', ' ', '|', ' '},
                {'-', '+', '-', '+', '-'},
                {' ', '|', ' ', '|', ' '},
                {'-', '+', '-', '+', '-'},
                {' ', '|', ' ', '|', ' '}};
        printGameBoard(gameBoard);
        Scanner keys = new Scanner(System.in);
        while (true) {
            System.out.println("Enter your placement (1-9) : ");
            int pos = keys.nextInt();
            while ( playerPositions.contains(pos) || cpuPositions.contains(pos)) {
                System.out.println("Position Taken! Enter a correct position : ");
                pos = keys.nextInt();
            }
            placePiece(gameBoard, pos, "player");
            Random rand = new Random();
            int cpuPos = rand.nextInt(9) + 1;
            while ( playerPositions.contains(cpuPos) || cpuPositions.contains(cpuPos)) {
                cpuPos = rand.nextInt(9) + 1;
            }
            placePiece(gameBoard, cpuPos, "cpu");
            String result = checkWinner();
            if ( result.length() > 0 ) {
                System.out.println(result);
                break;
            }
        }
    }

    public static void printGameBoard(char[][] gameBoard) {
        for (char[] row : gameBoard) {
            for (char c : row) {
                System.out.print(c);
            }
            System.out.println();
        }
    }

    public static void placePiece(char[][] gameBoard, int pos, String user) {
        char symbol = ' ';
        if (user.equals("player")) {
            symbol = 'X';
            playerPositions.add(pos);
        } else {
            symbol = 'O';
            cpuPositions.add(pos);
        }
        switch (pos) {
            case 1:
                gameBoard[0][0] = symbol;
                break;
            case 2:
                gameBoard[0][2] = symbol;
                break;
            case 3:
                gameBoard[0][4] = symbol;
                break;
            case 4:
                gameBoard[2][0] = symbol;
                break;
            case 5:
                gameBoard[2][2] = symbol;
                break;
            case 6:
                gameBoard[2][4] = symbol;
                break;
            case 7:
                gameBoard[4][0] = symbol;
                break;
            case 8:
                gameBoard[4][2] = symbol;
                break;
            case 9:
                gameBoard[4][4] = symbol;
                break;
            default:
                break;
        }
        printGameBoard(gameBoard);
    }

    public static String checkWinner() {
        List topRow = Arrays.asList(1, 2, 3);
        List midRow = Arrays.asList(4, 5, 6);
        List botRow = Arrays.asList(7, 8, 9);
        List lftCol = Arrays.asList(1, 4, 7);
        List midCol = Arrays.asList(2, 5, 8);
        List rightCol = Arrays.asList(3, 6, 9);
        List cross1 = Arrays.asList(1, 5, 9);
        List cross2 = Arrays.asList(7, 5, 3);

        List<List> winning = new ArrayList<>();
        winning.add(topRow);
        winning.add(midRow);
        winning.add(botRow);
        winning.add(lftCol);
        winning.add(midCol);
        winning.add(rightCol);
        winning.add(cross1);import java.util.List;
import java.util.Arrays;
import java.util.ArrayList;
import java.util.Scanner;
import java.util.Random;;
        public class TicTocToe {
            static ArrayList<Integer> playerPositions = new ArrayList<>();
            static ArrayList<Integer> cpuPositions = new ArrayList<>();

            public static void main(String[] args) {
                char[][] gameBoard = {{' ', '|', ' ', '|', ' '},
                        {'-', '+', '-', '+', '-'},
                        {' ', '|', ' ', '|', ' '},
                        {'-', '+', '-', '+', '-'},
                        {' ', '|', ' ', '|', ' '}};
                printGameBoard(gameBoard);
                Scanner keys = new Scanner(System.in);
                while (true) {
                    System.out.println("Enter your placement (1-9) : ");
                    int pos = keys.nextInt();
                    while ( playerPositions.contains(pos) || cpuPositions.contains(pos)) {
                        System.out.println("Position Taken! Enter a correct position : ");
                        pos = keys.nextInt();
                    }
                    placePiece(gameBoard, pos, "player");
                    Random rand = new Random();
                    int cpuPos = rand.nextInt(9) + 1;
                    while ( playerPositions.contains(cpuPos) || cpuPositions.contains(cpuPos)) {
                        cpuPos = rand.nextInt(9) + 1;
                    }
                    placePiece(gameBoard, cpuPos, "cpu");
                    String result = checkWinner();
                    if ( result.length() > 0 ) {
                        System.out.println(result);
                        break;
                    }
                }
            }

            public static void printGameBoard(char[][] gameBoard) {
                for (char[] row : gameBoard) {
                    for (char c : row) {
                        System.out.print(c);
                    }
                    System.out.println();
                }
            }

            public static void placePiece(char[][] gameBoard, int pos, String user) {
                char symbol = ' ';
                if (user.equals("player")) {
                    symbol = 'X';
                    playerPositions.add(pos);
                } else {
                    symbol = 'O';
                    cpuPositions.add(pos);
                }
                switch (pos) {
                    case 1:
                        gameBoard[0][0] = symbol;
                        break;
                    case 2:
                        gameBoard[0][2] = symbol;
                        break;
                    case 3:
                        gameBoard[0][4] = symbol;
                        break;
                    case 4:
                        gameBoard[2][0] = symbol;
                        break;
                    case 5:
                        gameBoard[2][2] = symbol;
                        break;
                    case 6:
                        gameBoard[2][4] = symbol;
                        break;
                    case 7:
                        gameBoard[4][0] = symbol;
                        break;
                    case 8:
                        gameBoard[4][2] = symbol;
                        break;
                    case 9:
                        gameBoard[4][4] = symbol;
                        break;
                    default:
                        break;
                }
                printGameBoard(gameBoard);
            }

            public static String checkWinner() {
                List topRow = Arrays.asList(1, 2, 3);
                List midRow = Arrays.asList(4, 5, 6);
                List botRow = Arrays.asList(7, 8, 9);
                List lftCol = Arrays.asList(1, 4, 7);
                List midCol = Arrays.asList(2, 5, 8);
                List rightCol = Arrays.asList(3, 6, 9);
                List cross1 = Arrays.asList(1, 5, 9);
                List cross2 = Arrays.asList(7, 5, 3);

                List<List> winning = new ArrayList<>();
                winning.add(topRow);
                winning.add(midRow);
                winning.add(botRow);
                winning.add(lftCol);
                winning.add(midCol);
                winning.add(rightCol);
                winning.add(cross1);
                winning.add(cross2);

                for (List l : winning) {
                    if (playerPositions.containsAll(l)) {
                        return "Congradulations you just WON! ";
                    } else if (cpuPositions.containsAll(l)) {
                        return "Sorry CPU wins ";
                    } else if  (playerPositions.size() + cpuPositions.size() == 9) {
                        return "Cat !";
                    }
                }
                return "";
            }
        }
        
