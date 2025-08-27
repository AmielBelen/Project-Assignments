# Programming Assignment 1  
My Programming Assignment 1 is explained in this repository.  

## Table of Contents  
- [Alphabet Soup Problem](#alphabet-soup-problem)  
- [Emoticon Problem](#emoticon-problem)  
- [Unpacking List](#unpacking-list)  

## Programming Assignments  
- [BELEN_PA1](./BELEN_EXPERIMENT%201_With%20Comments.ipynb)  

---

## Alphabet Soup Problem  
In this project, we are tasked to arrange the letters of a word in alphabetical order.  

I began by defining the function:  
```python
def alphabet_soup(text):
    # sorted() takes the input string and returns a list of characters sorted alphabetically
    sorted_letters = sorted(text)
    
    # join() combines the sorted list back into a single string
    print("".join(sorted_letters))
```

### Test Cases
```python
alphabet_soup("Programming101")       # Example with numbers and letters
alphabet_soup("AmielChristianAjedoBelen")  # Example with mixed upper/lowercase
alphabet_soup("TestNumber3")
```

---

## Emoticon Problem  
In this project, we are tasked to change words into emoticons. Specifically, the smile, grin, sad, and mad emoticons.  

I began by making the function needed that would replace the keywords with their emoticon equivalents:  
```python
def emotify(emote):
    # Convert the input to lowercase so it works regardless of capitalization
    emote = emote.lower()
    
    # Replace specific words with their emoji equivalents
    e = emote.replace("smile", ":)")
    e = e.replace("grin", ":D")
    e = e.replace("sad", ":(")
    e = e.replace("mad", ">:(")
    
    # Print the final transformed string
    print("Emotified:", e)
```

### Test Cases
```python
emotify("That show always makes me SMILE")  
emotify("I always feel sad when I don't have high grades")  
emotify("Try to grin and smile instead of being mad")  
```

---

## Unpacking List  
In this project, we are tasked to split a collection of numbers into three variables: first, middle, and last.  

I began by creating a sample list first:  
```python
numbers = [25, 14, 1, 7, 8]
```

Then, I unpacked the list:  
```python
first, *middle, last = numbers
print("First:", first)
print("Middle:", *middle)
print("Last:", last)
```

