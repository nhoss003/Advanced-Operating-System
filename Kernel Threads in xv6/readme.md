Adding real kernel threads to xv6. 
======================================

1- Defined a new system call to create a kernel thread, called clone().

2- Used clone() to build a little thread library, with a thread_create() call and lock_acquire() and lock_release() functions.

3- wrote a test program in which multiple threads are created by the parent, and each insert items into a thread-safe linked list.
