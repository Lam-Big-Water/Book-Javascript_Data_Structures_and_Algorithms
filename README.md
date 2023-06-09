# Book-Javascript_Data_Structures_and_Algorithms


## Interesting Question

```javascript
console.log('Sam' ? true : false);
//output: true.
```

Now, what about the following code ? Let's take a look:

```javascript
console.log('Sam' == true);
//output: false.
```

The output is **false**, so let's understand why:

- First, it converts the boolean value using **toNumber**, so we have **Sam == 1**.
- Then, it converts the string value using **toNumber**. Since the string consists of alphabetical characters, it returns **NaN**, so we have **NaN == 1**, which is false.

What about the following code ? Let's take a look:

```javascript
console.log('one' == false);
//output: false.
```

The output is also **false**, and the following is why: 

- First, it converts the boolean value using **toNumber**, so we have **one == 0**.
- Then, it converts the string value using to **toNumber**. Since the string consists of alphabetical characters, it returns **NaN**, so we have **NaN == 0**, which is false.