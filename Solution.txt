class Solution
{
    static void Main(string[] args)
    {
        Console.WriteLine("Enter your text(Press the 'q' key to exit): ");

        string input = "";
        string input1;

        while ((input1 = Console.ReadLine()) != "q")
        {
            input += input1 + Environment.NewLine;
        }
        
        string[] lines = input.Split("\n");
        Console.WriteLine("Output: ");

        foreach (string line in lines) {
            string[] words = line.Split(' ');
            Array.Reverse(words);
            Console.WriteLine(string.Join(" ", words));
            }
    }
}