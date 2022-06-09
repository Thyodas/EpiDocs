---
description: How are stumpers graded?
---

# 📈 Grading

{% hint style="danger" %}
This part is really important as it lists everything you have to do to avoid any surprise during your stumper.
{% endhint %}

Solo stumpers are only graded by the automated tests. If you pass 15/20 tests you pass the stumper and you'll be eligible to take duo stumpers.

Duo stumpers are graded by the automated tests too. If you pass 15/20 tests you are eligible for the defense that takes place after the exam. This page will help you pass this defense as it can be sometimes tricky.

### So, what should I check then?

| Bad Behavior                             |                                                Penalty                                               |
| ---------------------------------------- | :--------------------------------------------------------------------------------------------------: |
| Mallocs not checked                      |                                               Undefined                                              |
| Norm (manually or automatically checked) |    Minor <mark style="color:orange;">**-1**</mark> / Major <mark style="color:red;">**-3**</mark>    |
| Relink                                   |                                <mark style="color:red;">**-5**</mark>                                |
| -g in production Makefile                |                          <mark style="color:red;">**-4**</mark>** ** per -g                          |
| No .PHONY in Makefile                    | <mark style="color:orange;">**-1**</mark>** **<mark style="color:blue;">****</mark> per missing rule |
| Valgrind Errors                          |                              **-**<mark style="color:red;">**5**</mark>                              |
| Memory Leaks                             |          <mark style="color:orange;">**-3**</mark> to <mark style="color:red;">**-5**</mark>         |
| Missing static keyword on functions      |                                               Undefined                                              |
| Crash                                    |                                <mark style="color:red;">Failed</mark>                                |
| Banned functions                         |                                <mark style="color:red;">Failed</mark>                                |
| Cheating                                 |                                <mark style="color:red;">Failed</mark>                                |

{% hint style="warning" %}
The sum of all these penalties and the results of your automated tests must be above or equal to 15/20 if you want to pass.
{% endhint %}

