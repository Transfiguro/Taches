# Taches
Short description:
Taches, shedule yourself tasks, messages and programs to be run when you want or when Windows starts.

Long description:
Managing programs started when you start your computer is doing what Windows can not do, specifically:
-control the order in which they launch,
-control their frequency of execution (they are not all obliged to run at each start),
-if necessary, give the user the choice to launch them or not,
-wait for the end of the execution of a program before launching another one or, on the contrary, launch one without waiting for the previous one to be finished.
In short, it's really all master of these Windows session start programs. That's what Taches does.

There are probably several tasks that you have to perform regularly on your computer, such as backing up, cleaning your disk, or scan it for malwares. For example, you may have decided to start a backup program every three days, but without taking into account the days when the computer was stopped - and that's what changes everything - because you went on weekend or vacation. Indeed, there was nothing to save those days. How to do this thing automatically with your computer?

The Windows Task Scheduler does not allow it. I do not believe that any existing software is capable of it. That's why I wrote Taches, a small portable freeware, simple and yet powerful, which allows:
-to launch a program, a command, or to display a message,
-to launch a program, an order, or to display a message, every n days,
-to launch a program, a command, or to display a message, every n days without counting the days when Windows was not started.

For example, suppose that you want to make a backup every three days of actual work on the computer. You make one on a Thursday. You work the next day, Friday. Then you go on a weekend. You do not start your computer on Saturday or Sunday. You use it again on Monday. Tuesday, it will be three days worked since the last backup: Friday, Monday, and Tuesday. You should make a backup on Tuesday. Taches will take care of counting the number of days you start the computer, and start the right action when the desired number of days is reached.

Another example: you clean your drive every ten days. One day, you go on vacation just after doing it. When you come back from your holidays, certainly deserved, must the disk be cleaned? No, of course, because everything happens as if, for the computer, you had done it the day before. It will have to be done in ten days. Taches will be able to launch the defragmentations for you, if, of course, you have installed a defragmentation software.

These different actions are described in a text file, named Taches.txt, which is in the Taches folder, and that is created the first time that you run Taches.exe, with an action as an example to modify. With a text editor, like Windows Notepad, notepad.exe, you can add as many actions as you want, putting one action per line, and respecting the correct syntax (see the example). Lines that begin with ' are comments and are ignored by Taches.

The benefits of Taches are:
-Planning of repetitive tasks to be done every n days.
-Small, without installation.
-Do not install service. It runs then goes out or goes to sleep, so it does not occupy the system permanently.
-The tasks are easy to configure. A simple text editor is enough.
-The tasks are executed one after the other. A task is started immediately or when the previous task is completed, as desired.
-Runs silently, just starting the tasks or displaying the requested messages.
-But, in case of syntax error, it signals the line number where the error is.
-Can be used to launch several programs in a certain order, just by running it once. This is done by creating a new copy of the Taches folder, and editing a simple text file.
-You can use absolute or relative paths. This allows the program to run correctly with portable devices, when the drive letter can change.
-You can play sounds.
Taches runs silently and tests each line to see whether to launch it or not.
