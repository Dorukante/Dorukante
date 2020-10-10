public class FibonacciSequence {
    int CurrentNum;
    int Previousnum;
    int Sum;

    public void Run() {
        Previousnum = 1;
        CurrentNum = 1;
        for(int i = 0; i < 100; i++) {
            Sum = Previousnum + CurrentNum;
            Previousnum = CurrentNum;
            CurrentNum = Sum;
        }
        System.out.println(Sum);
        }
    
    public static void main(String[] args) {
        FibonacciSequence runner = new FibonacciSequence();
        runner.Run();
    }

}



