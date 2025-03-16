# Basic Features of MonkeyLang

## **1. Variables**  
Declare variables using `create variable`:

```monkeylang
create variable name as "MonkeyLang"
create variable age as 2
```

## **2. Conditionals (if-else)**  
Use `if-else` statements for decision-making:

```monkeylang
if age is greater than 1 then
    show "MonkeyLang is growing!"
else
    show "Just getting started!"
end
```

## **3. Loops**  
Use `while` and `for` loops:

```monkeylang
create variable count as 0

while count is less than 5 do
    show "Looping..."
    increase count by 1
end
```

## **4. Functions**  
Define reusable functions using `create function`:

```monkeylang
create function greet with parameter name
    show "Hello " + name
end

call greet with "User"
```

## **5. Input/Output**  
- Show messages using `show`:
  ```monkeylang
  show "Welcome to MonkeyLang!"
  ```
- Get user input:
  ```monkeylang
  create variable username as get input "Enter your name: "
  show "Hello " + username
  ```
