# Interface

# Aim:
To Develop a small bank application by declaring deposit() and withdrawal() as abstract methods in the interface. Get the choice from the user whether to perform withdrawal or deposit operation. After the operation completes, display the balance amount

# Algorithm:

Step 1: Create an interface.

Step 2: Create a child class.

Step 3: Declare 2 functions deposit() and withdrawal() as abstract methods in the interface.

Step 4: Create those 2 functions in the child class and perform respective operation.

Step 4: Use if-else conditional statement to get the choice from the user whether to perform withdrawal or deposit operation.

Step 5: After performing the functions display the remaining balance of the user.

# Program:

Name: HARITHASHREE.V
REG.NO.: 212222230046
```python
using System;
public interface Bank
{
    void deposit();
    void withdrawal();
}
class Program : Bank
{

    int amount, ch, balance = 2000;
    public Program()
    {
        Console.WriteLine("1.Deposit\n2.Withdrawal");
        ch = Convert.ToInt32(Console.ReadLine());
        if (ch == 1)
        {
            deposit();
        }
        else
        {
            withdrawal();
        }

    }
    public void withdrawal()
    {
        int amount = Convert.ToInt32(Console.ReadLine());
        balance -= amount;
        Console.WriteLine(balance);
    }
    public void deposit()
    {
        int amount = Convert.ToInt32(Console.ReadLine());
        balance += amount;
        Console.WriteLine(balance);
    }

}
class example
{
    public static void Main()
    {
        Program c = new Program();
        c.deposit();
        c.withdrawal();
    }
```


# Output:

![image](https://github.com/haritha-venkat/Interface/assets/121285701/0aaa50d0-15dd-4059-819d-735eabb04355)


## Result:
Thus, a C# program was developed for a bank application using interface.


