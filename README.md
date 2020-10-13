# cl-cron

A simple tool that provides cron like facilities directly inside of common lisp.

a fork of https://bitbucket.org/mackram/cl-cron (unavailable)

Install with Quicklisp:

    (ql:quickload "cl-cron")

Note: Quicklisp does not point to this repository.

Example:

Print a message every minute.

~~~lisp
  (defun say-hi () (print "Hi!"))
  (cl-cron:make-cron-job #'say-hi)
  (cl-cron:start-cron)
~~~

Wait a minute to see output.

Stop it with `stop-cron`.

## API

http://quickdocs.org/cl-cron/api

Licence: GPL