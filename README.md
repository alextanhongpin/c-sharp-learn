# learn-c-sharp
Learning C#
```c#
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;


namespace SoloLearn
{
    class Program
    {
        static void Main(string[] args)
        {
            int myInt = 1;
            float myFloat = 1f;
            bool myBool = true;
            string myName = "john";
            string emp = String.Empty;
            char myChar = 'a';
            double myDouble = 1.75;
            if (myBool) {
                Console.WriteLine("this is true");
            }
            List<int> nums = new List<int>(){1,2,3,4};
            var newNums = nums.Select(i => i * 2);
            nums.Add(100);
            nums.Remove(4);
            Console.WriteLine(nums.Count);
            
            foreach (int i in nums) {
                Console.WriteLine(i);
            }
            foreach (int i in newNums) {
                Console.WriteLine(i);
            }
            
            Dictionary<string, int> ids = new Dictionary<string, int>();
            ids.Add("Car", 110);
            if (ids.ContainsKey("Car")) {
                Console.WriteLine(ids["Car"]);
            }
            ids.Remove("Car");
            Console.WriteLine(ids.Count);
        }
    }
}
```
