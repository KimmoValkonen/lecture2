# Activities

## Task 1/5

> Refer to the instruction in [GitHub Workflow](../github.md)

- Clone today's repo
- Create a new branch e.g answers
- Create a repository in GitHub
- Change remote to point to your repo

## Task 2/5: Brute force

- What is the maximum number of steps it would take to perform a linear search on an ordered array of size 100,000?
  > Refer to `./src/search-linear.cpp`
# Answer: 100,000 steps

## Task 3/5: Decrease-and-Conquer

- What is the maximum number of steps it would take to perform a binary search on an ordered array of size 100,000?

  > Refer to `./src/search-binary.cpp`
  # Answer: 17 steps

## Task 4/5: Quiz

32 teams qualified for the 2014 World Cup. If the names of the teams were arranged in sorted order (an array), how many items in the array would binary search have to examine to find the location of a particular team in the array, in the worst case?

- [] At most, 32.
- [] At most, 1.
- [x] At most, 6.
- [] At most, 16.

## Task 5/5: Individual, at home

Refactor the code in `./src/task4.cpp` to use recursion

- Refer to the following [link](https://www.techiedelight.com/binary-search/)
- Make sure that you:
  - Replace `printf()` with` std::cout()`
  - Include the right headers e.g. `iostream`
  # Answer: I used `using namespace std;` instead of `std::cout()`
  # the code is below and results: `Element found at index 1`

  #include <iostream>

using namespace std;

int binarySearch(int nums[], int low, int high, int target)
{
							  
    if (low <= high)
    {
        int mid = (low + high) / 2;
        if (target == nums[mid])
        {
            return mid;
        }
        else if (target < nums[mid])
        {
            return binarySearch(nums, low, mid - 1, target);
        }
        else
        {
            return binarySearch(nums, mid + 1, high, target);
        }
    }
    return -1;
}

int main()
{
    int nums[] = {2, 5, 6, 8, 9, 10};
    int target = 5;
    int n = sizeof(nums) / sizeof(nums[0]);
    int index = binarySearch(nums, 0, n - 1, target);
    if (index != -1)
    {
        cout << "Element found at index " << index << endl;
    }
    else
    {
        cout << "Element not found in the array" << endl;
    }
    return 0;
}


## Links

- https://cpp.sh/
- https://www.techiedelight.com/binary-search/
- https://www.softwaretestinghelp.com/searching-algorithms-in-cpp/
- https://www.khanacademy.org/computing/computer-science/algorithms/binary-search/e/running-time-of-binary-search


