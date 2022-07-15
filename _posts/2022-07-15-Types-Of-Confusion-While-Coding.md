---
layout: post
title: Types of Confusions While Coding
categories: [Programming]
---
There are 3 types of confusion in coding.

## 1. Lack of Knowledge  
Issues in long term memory. 
### Example
If you don't know lisp, then this code would be hard to read and understand.  
```clojure
(defun timed-notification()
  (interactive)
  (let ((msg "Take a break, time's up!"))
    (run-at-time 25 nil (lambda (mess) (terminal-notifier-notify "pomodoro" mess)) msg)))
``` 
There is code that you don't know the language. You can learn it but, it will take long time if it is not like other languages you already know. E.g. a prolog or lisp code.
### Solution
- Learn it, then use spaced repetition apps like anki to keep your programming knowledge.
- Check cheat sheets of the of topic you want to learn. To find cheat sheets, google "[subject] cheat sheet". E.g. "Lisp cheat sheet"

## 2. Lack of Information  
Issues in short term memory.  
### Example
```python
def main():
    arr = [-4, 1, 4, 10, -10, 4, -3]
    arr.sort()
    print(arr)
```
It is obvious that it sorts the array, but you may not know what algorithm it uses and if it is in-place or not.  
### Solution
- I have made a web app for [short term memory](https://github.com/mertserezli/ShortTermMemorization). If you have to retain it for a few days, you can use it.
- Challenge yourself with small snippets of code. Check a code and rewrite it from memory.  
- If it is something you won't need in the future, you can google it.
- Play dual n-back from time to time to train your short term memory. Some researchers say it works and some say it doesn't work.  

## 3. Lack of Processing Power
Issues in working memory. 
### Example
```python
def f(m,n):
    if m < n:
        (m,n) = (n,m)
    while (m % n != 0):
        (m, n) = (n, m % n)
    return n
```
There is a code that has lots of variables and does lots of things with these variables. 
This is the euclidean algorithm to find the greatest common divisor. It is hard to understand if you don't know it already.   
### Solution
Try to run it with pen and paper. 

## Conclusion
You may have encountered these types of issues in your coding career, but didn't know what's wrong or what to do. With these tools and techniques, you can solve these issues.