using System;
using System.Collections.Generic;
using System.Diagnostics;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Pennies
{
    internal class Change
    {
        public int Pennies { get; }
        public int Nickels { get; }
        public int Dimes { get; }
        public int Quarters { get; }
        public int HundredDollarBills { get; }
        public int FiftyDollarBills { get; }
        public int TwentyDollarBills { get; }
        public int TenDollarBills { get; }
        public int FiveDollarBills { get; }
        public int DollarBills { get; }

        static void Main(string[] args)

        {
            Console.WriteLine("See I'm Here.");

            Console.ReadKey();
        }

        public class Change_Blueprints
        {
            public int HundredDollarBills { get; }
            public int FiftyDollarBills { get; }
            public int TwentyDollarBills { get; }
            public int TenDollarBills { get; }
            public int FiveDollarBills { get; }
            public int DollarBills { get; }
            public int Quarters { get; }
            public int Dimes { get; }
            public int Nickels { get; }
            public int Pennies { get; }



        }
        public Change(decimal price)
        {
            HundredDollarBills = (int)(price / 100);
            price %= 100;

            FiftyDollarBills = (int)(price / 50);
            price %= 50;

            TwentyDollarBills = (int)(price / 20);
            price %= 20;

            TenDollarBills = (int)(price / 10);
            price %= 10;

            FiveDollarBills = (int)(price / 5);
            price %= 5;

            DollarBills = (int)(price / 1);
            price %= 1;

            Quarters = (int)(price / .25m);
            price %= .25m;

            Dimes = (int)(price / .10m);
            price %= .10m;

            Nickels = (int)(price / .05m);
            price %= .05m;

            Pennies = (int)(price / .01m);

            Console.ReadKey();  
        }
        
    }
    }

