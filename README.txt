#Demo Git Repository
This s the first try of commiting in git.


##Ipsum Below
When we implemented the git portion of Sublime Merge, we chose to use mmap for reading git object files. This turned out to be considerably more difficult than we had first thought. Using mmap in desktop applications has some serious caveats, and here's why:

You can follow along with the example project here.

Say you were reading some binary format, data you need throughout some application. You take the easiest approach and use a simple read to get the full contents of the file. You release your software and someone comes along and says: "I need to parse this 3GB file, but I only have 2GB of memory. Could you make it so that you're not using so much memory?". Of course you want to help them, so you do some searching and come to the conclusion that memory mapping is the perfect solution to this problem.