# Node.js Test
write a NodeJS function that will process N number of tasks concurrently, until the taskList
is exhausted. N defines the number of concurrent promises that your script should attempt to resolve, and
should be changeable on the fly. For example, if the current local time is between 9am and 5pm, N = 10,
otherwise N = 150.
It is very important to note that promises must be processed in parallel, such that if N = 10, then there are
always 10 promises being resolved (e.g. API requests). When one finishes, another immediately starts. It
is not acceptable to resolve 10 promises, wait until all 10 have resolved, and then begin another 10.
For example, if N = 3, then you will execute 'A', 'B', and 'C' in the taskList concurrently. Once B
finishes, you then execute 'D', and so on.
Restrictions: Use pure NodeJS (JS or TS) with no external libraries/dependencies at all allowed.

