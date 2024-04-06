# About [Me](/images/Headshot.jpg)

Hi! I'm **Jason**, and I'm a 3rd year Math-CS student in CSE 110 for Spring 23-24. I'm excited to learn all about what this course has to offer, whether it's from Professor Powell, my classmates, the resources available, or myself! If I were to describe myself with a quote, it would be:
>"That's my favorite saying" -[~~Lebron~~ My Glorious Sunshine](https://www.youtube.com/watch?v=de_RFVywzO0)

## Personal Interests

### Hobbies (*in order of prevalence*)

  1. Basketball
  2. Volleyball
  3. Cooking/Baking
  4. Videograpgy
  5. Video Games
  6. Drawing
  7. Surfing

### Favorites

- **Food**: Sweet baked goods
- **Music Artists**: A$AP Rocky, Slowdive, Deftones, Soulja Boy, T-Pain just to name a few...
- **Movie**: Everything Everywhere All at Once
- **Show**: ATLA
- **Youtube Channel**: Whichever uploads longest European Football match highlights

## Programming

Most if not all of my programming experience comes down to the courses I've taken from high school and university through now. I've only recently become more passionate (*and gotten over my perfectionism paralysis*) and taken the initiative to learn outside of my studies. I'm still not sure what direction/specialization I want to move towards, so my main priority is learning what I don't know and what I don't know that I don't know.

### Some Relevant Knowledge

- Languages: Java, C, C++, SQL, HTML, CSS, JavaScript
- Basic to Intermediate Algorithms and Data Structures
- Object Oriented Design
- Basic Systems Programming
- Computational math and analysis

### Proudest Leetcode Solution

```Java
class Solution {
    public int minSwaps(int[] nums) {
        int totalOnes = 0;
        for (int i : nums) {
            if (i == 1)
                totalOnes++;
        }
        int[] newNums = new int[nums.length*2];
        System.arraycopy(nums, 0, newNums, 0, nums.length);
        System.arraycopy(nums, 0, newNums, nums.length, nums.length);        
        int windowCount = 0;
        for (int i = 0; i < totalOnes; i++) {
            if (newNums[i] == 1) {
                windowCount++;
            }
        }
        int max = windowCount;
        int start = 0;
        for (int i = totalOnes; i < newNums.length; i++) {
            if (newNums[i] == 1) {
                windowCount++;
            }
            if (newNums[start] == 1) {
                windowCount--;
            }
            max = Math.max(max, windowCount);           
            start++;
        }
        return totalOnes-max;
    }
}
```

## Fun Facts

- Born in Orange County, CA, Moved to Utah when I was 2, moved back to Orange County, CA when I turned 5, living there ever since
- 4 years varsity Basketball and Volleyball
- Dogs > Cats
- Die hard L(ebron)aker fan
- I met the entire Ball Family

### Places I've traveled to/lived in (and want to)

- [x] Vietnam
- [x] China
- [x] Hawaii
- [x] All of California
- [x] Utah
- [ ] France
- [ ] Italy
- [ ] England
- [ ] Japan
- [ ] Korea
- [ ] Alaska
- [ ] Iceland
- [ ] Australia
