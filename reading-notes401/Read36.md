# Whiteboard Advice
Whiteboard-style interviews are ubiquitous in the tech industry. For those who not had the pleasure, whiteboard interviewing is the practice of asking candidates to solve technical questions on a whiteboard, piece of paper, or computer during the interview. This kind of environment can feel like a pressure cooker and cause even the most competent engineer to fall apart.

The best piece of technical interview advice I have received and can impart upon you is to communicate, communicate, communicate! This may seem like an anti-climactic piece of advice, but I hope to be able to demonstrate to you that it’s actually the most important skill to prepare prior to an interview.


## 7 tips to ace a programming interview
1. Take a few minutes.
Speaking as an interview coach, this is one misstep that I see all the time during mock interviews. The canonical tip that everyone gives is, “talk more!”. What most of those well-meaning advice-givers overlook, however, is that talking and thinking at the same time is extremely hard. Nervous interviewees will jump straight into talking, passing up a great opportunity for concentrated thought.

2. Write down the steps of the solution.
Even after you have an idea of how to attack the problem, don’t start writing code down. Write down the general steps of how you will solve it on one side of the whiteboard, where it’s visible but won’t get in the way. You don’t need to be verbose, just get the steps in order and somewhat readable.
- Start at middle of array.
- Keep variables tracking left and right boundaries of search area.
- If value equal to search_val, return true.
- If left and right boundaries are adjacent, return false.
- If value bigger than search_val, go halfway towards left boundary, and move the right boundary along with us.
- If value smaller than search_val, go halfway towards right boundary, and move the left boundary along with us.

3. Write pseudocode first.
Time to write code? Nope. Take a “dry run” at writing the code by writing some pseudocode. Often we run into problems halfway through writing the code, and there’s no point wasting time over syntax when you might have to throw the code away. Instead, write some half-baked code-looking stuff that lays out the structure of how your code will work. Do it over on the side of the whiteboard, so you have space left to work.

4. Don’t sweat the small stuff.
Programming interviews are not about how well you’ve remembered your semicolons, nor are they about being able to remember all of the flags on a TCP packet. They’re about demonstrating depth and breadth of knowledge, personality strengths, and problem-solving abilities. If you make a mistake, it’s okay. Brush it off and move on.

5. Sit down. Be humble.
A programming interview isn’t just a written exam. It’s an assessment of your programming abilities, and there are plenty of things that fall into that category beyond mere coding prowess. For example:
- Are you able to express your ideas and solutions clearly and effectively?
- Do you treat the interviewer with respect?
- How do you accept criticism (technical, constructive or otherwise)?
- Are you able to collaborate with others to come up with solutions?
- Do you communicate in a way that demonstrates empathy?
- Are you honest (especially about yourself)?

6. Come prepared.
When it comes to programming interviews, there is no substitute for HOBIS (which stands for Hours of Butt-In-Seat). If you want to be ready, you have to put in the time. It’s important in order to maximize your chances of acing the interview, but it’s also important for your peace of mind during the interview and afterwards. In the interview, knowing that you’ve done all you can to prepare helps you stay calm and cool, and increases your chances of success. And afterwards, regardless of the outcome, knowing that you could not have reasonably done more to prepare helps you feel proud of your work and start moving towards your next goal.

7. Review your work.
You won’t always finish questions in the time permitted, but occasionally you’ll have extra time after coming up with a solution. If this happens, it’s tempting to say “Well, I’m done!”. Interviews are stressful and we want them to be over as fast as possible.  
**focus on these two areas, as they receive heavy scrutiny in interviews:**
1. **Algorithmic efficiency**. Have you found the fastest and most optimal solution given the requirements? Take some time and consider other approaches. It’s worth noting two things here: 1) If the problem involves a sorted dataset, you can bet your pants there’s a solution involving ` O(log(n)) lookup time (even if there’s additional cost, the total complexity will still contain the log(n), for example, O(n * log(n)) if iterating over an array, as sorting algorithms do), and 2) For a disgustingly large number of programming interview questions, the answer involves a hash table and O(1) lookup time — so if you’re seeking a better algorithm, try a hash table.
1. **Correctness**. Sure, you’ve solved for the simple, easy use case, but have you checked for edge cases? Off-by-one errors? Issues with negative numbers or empty arrays or missing keys or strings with weird patterns of characters? Maybe you won’t find all of them, but failing to at least LOOK for edge cases before declaring your solution to be correct is a pretty hefty mistake in an interview.
