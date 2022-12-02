# Data Structures

**What is 1 of the more important things you should consider when deciding which data structure is best suited to solve a particular problem?**

When considering which DS to use for solving a certain problem it is important to consider: The size of the data you are working with and how you intend to manipulate it. Because if the size of the data is not really too big than certain data structures might be too over kill or of course if the size of the data is really big than you would need more control and more effenctincey when it comes to look up certain pieces of the data. The next mentioned thing to consider is what the use case is, if you are looking to "find" a specific piece of data on a large scale project that requires one to find a specific piece of data than using a DS that uses "keys" in order to find the specific peice of data can be helpful, or maybe you need to add or delete said pieces of data, trying to add to that existing data structure can create problems in memeory if the data structure itself becomes to big, which may mean it has to be moved or it can also suffer a "collision".

**How can we ensure that we’ll avoid an infinite recursive call stack?**

This can be "taken care of if we utilize the two case system. the "base case" and the "Recursion case" the base case is the almost like the "initialization" where we could set the condition and even set our return for if the condition is met then we could return from that function. If that condition is not met than we would call that function on itself until that condition gets met. This would obviously beat the lack of the base case which would than creat an infinite loop.
