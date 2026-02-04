# To-Do List App

Made this because I kept forgetting stuff I needed to do. Post-it notes were getting out of hand and I lose my phone notes all the time, so figured a simple command line thing would be easier.

## What's it for

Basic task manager that runs in your terminal. Add tasks, remove them when you're done, see what's on your list. Nothing fancy but it gets the job done.

## Running it

Just need Python:
```bash
python todo_list.py
```

Menu shows up with options 1-4. Pick what you want to do.

## The options

**1. Add task** - Type in whatever you need to remember and it gets added to your list

**2. Remove task** - Type the exact task name to delete it (has to match perfectly or it won't find it)

**3. Show tasks** - Prints out everything on your list with bullet points

**4. Quit** - Exits the program

## Example usage

```
1.add task
2.remove task
3.show task
4.quit
Enter your choice: 1
Enter task: buy groceries
Enter your choice: 1
Enter task: call mom
Enter your choice: 3
Tasks: 
- buy groceries
- call mom
Enter your choice: 2
Enter task to remove: buy groceries
Enter your choice: 3
Tasks: 
- call mom
Enter your choice: 4
```

## Problems I'm aware of

There's some obvious issues that I just haven't fixed yet:
- Tasks don't save anywhere, so when you close the program everything's gone
- That `from random import choice` at the top literally does nothing, copied it from another file and forgot to delete it
- Have to type the task name exactly right to remove it, even one letter off and it won't work
- No way to edit a task, you have to delete and re-add it
- Empty task list doesn't show any special message, just says "Tasks:" with nothing under it

## Why it's like this

Honestly I threw this together in like 15 minutes when I needed something quick. Could've made it way better but this covers my basic needs. Sometimes the simplest solution is good enough right?

## Things I might add later

If I ever come back to this (probably won't but who knows):
- Save tasks to a file so they persist between runs
- Mark tasks as complete instead of just deleting them
- Add due dates or priorities
- Search/filter tasks
- Better matching for remove (like partial text search)
- Some color coding maybe
- Edit existing tasks without deleting

But realistically I'll probably just use this as-is until I get annoyed enough to fix something.

## Code notes

Pretty straightforward Python:
- Everything's in one function which isn't great practice but whatever
- Uses a list to store tasks in memory
- Basic menu loop with if-elif statements
- The remove function checks if task exists first which is good

Not the cleanest code I've written but it works. Sometimes that's all that matters.

## For beginners

If you're learning Python this is actually a decent starter project. Shows you:
- Functions
- Lists and list methods (append, remove)
- While loops
- User input
- Basic menu systems
- If-elif-else logic

Not too complicated but covers useful concepts.

---

Use it however you want. Improve it, break it, learn from it, whatever works for you. No license or anything, it's just a simple script.
