A2 kit: CPU scheduling in xv6 (MLFQ)
====================================

Two folders, each laid out like the xv6 repo (Makefile, kernel/, user/):

  skeleton/   everything is done EXCEPT your two tasks, which are marked
              with TODO comments in kernel/proc.c. start with this one.

  solution/   the same files, completely finished and tested.
              only kernel/proc.c is different from the skeleton.

Start (fresh clone, then copy the skeleton over it):

  git clone https://github.com/guanslab/xv6-a1-starter.git ~/xv6-a2
  cp -r ~/Downloads/ai-code/a2-kit/skeleton/. ~/xv6-a2/
  cd ~/xv6-a2
  make CPUS=1 qemu

If you get stuck or run out of time, drop in the finished file:

  cp ~/Downloads/ai-code/a2-kit/solution/kernel/proc.c ~/xv6-a2/kernel/proc.c

Tests (inside xv6):

  make CPUS=1 qemu   then:  pinfotest        (part 1)
                            mlfqtest         (part 2, about a minute)
  make qemu          then:  mlfqtest stress  (3 cpus)
                            usertests -q     (about 5 minutes)

The step-by-step guide with hints is A2-Guide-and-Hints.docx.
The answers are in A2-Answer-Key.docx.
