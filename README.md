# pintos-threads

Academeic Project at LNMIIT as a part of Operaing Systems (2015) Course, offered to B.Tech. 5th sem. students.

*About:*

Pintos kernel supports multiple in-kernel threads. It already includes code for initialization, thread creation and destruction, context switches, thread blocking and unblocking as well as a simple but preemptive round-robin scheduler. In this project, we implement several features that exercise thread state transitions. This project shows how the illusion that “computers can do multiple things at once” is created by a sequence of thread state transitions and context switches. Moreover, this also shows how sophisticated scheduling policies can be built on top of a simple priority-based scheduler.

*Modules:*

  * Part I – **Alarm Clock:** In this module we maintain a timer queue of sleeping threads and changing the timer interrupt handler to unblock those threads whose wakeup time has arrived. This involves protecting threads that are shared between a thread and an interrupt handler.

  * Part II – **Priority Scheduler:** This module constitutes a strict priority-based uniprocessor scheduler. 

  * Part III – **Priority Inheritance:** Based on the priority scheduler, we also implement priority inheritance. This is to protect from priority inversion.

  * Part IV – **Multi-Level Feedback Queue:** Separately, we build a multi-level feedback queue scheduler on top of the strict priority scheduler. This scheduler adjusts threads’ priorities based on a sampling of how much CPU time a thread has received recently.
