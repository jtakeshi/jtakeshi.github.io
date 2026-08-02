---
title: 'Research programming tips from my time at Notre Dame'
date: 2025-08-25
permalink: /posts/2025/08/programming-tips/
tags:
  - programming
  - from_nd
---

(These were originally written during my time as a graduate student. After a bit of time and perspective, I should note that this is tailored to the kind of research that I do, and also to my personal way of doing things, which has worked for me well in the past and hopefully is useful to students at some point. The wise student also knows when and how to ignore these guidelines. A more full description of my programming guidelines for my research group is in progress and should be available Soon(TM).)

A collection of miscellaneous programming and computer tips that I really needed at some points in the past, and probably will need again in the future.

- Keep it simple, stupid.
  - Program exactly what you mean, and optimize later. (But don’t write lazy slow code on the first run either!)
  - Don’t use language features just because they exist (e.g., C++ templates).
  - Use boring, battle-tested tools and software. People have been trying for decades to replace C and C++; don’t be a guinea pig in the latest attempt.
- Use the right tool for the job, and be willing to learn new tools as the job requires. Be flexible.
  - Python is best for gluing other stuff together, and getting something up and running quickly.
  - C++ can do, or be used for, pretty much anything. This is not always a good thing.
- Learn C. No way around it.
- Learn the const keyword, in all its incarnations, and use it wherever possible.
  - Pass by const reference for anything significantly larger than a word (usually 64 bits).
  - Declare class functions const as appropriate. If this causes a lot of compiler errors, you’re doing something wrong.
- Test thoroughly. Testing is what demarcates engineering and scratch work.
- Learn the Linux toolchain and other tools. Even just a few tricks with gcc, bash, git, gdb, valgrind et al. can go a long ways. Especially git.
- Use Linux as a daily OS – I recommend Ubuntu or Pop_OS. It’s actually easier to get things done in Ubuntu than in Windows nowadays.
- Ensure a bijection exists between calls to malloc/calloc/new and calls to free/delete.
  - Write the allocation, write the deallocation immediately after, then write your code in between those lines.
  - Also, make sure the correct number of bytes (hint: use sizeof) are argued to malloc/calloc, and check the returned pointer.
- Write functions to return error codes, and check those returned values.
- Use preprocessor macros to create a debug build.
- The tougher the task, the more assertions you should have – 1:8 was the recommended ratio of assertions to lines of code for my undergraduate operating systems course.
- Also, macros are a must-know for any cross-platform programming.
- Have a complete and clear specification for the project, and do not try to add in features a week before the deadline.
- Start the project when it is assigned, and don’t procrastinate, unless you want to have a segfault you can’t figure out on the due date. This is harder for research projects where the goals and scope may frequently change.
- Only keep one copy of a program installed on your system.
  - Python is the worst offender, but the 2/3 split isn’t always easily resolved.
- Never hardcode values – it makes debugging harder, and makes bugs easy. Use static const (C++) or #define (C) for constants.
- Mount your home and root directories on different disk partitions, so that you can easily switch operating systems while keeping your files.
- Keep Windows and Linux on different disks so the Windows updater can’t mess with the Linux partitions.
- Learning to use /etc/fstab to manage your disks and partitions will be time very well spent.
