# WIX1002_W02_Tutorial_1
### 📃 Question 1
#### 📊 IPO Model
| Input | Process | Output |
|----------|----------|----------|
| - Number_1  <br> - Number_2 | Multiple number_1 and number_2 | Product of number_1 and number_2
|
#### 💻 Pseudocode
```text
START 
    Read number_1, number_2
    product =  number 1 * number 2
    Display product 
END
```
#### 🧮 Flow Chart

![Flowchart for question 1](Q1.png)



### 📃 Question 2
#### 📊 IPO Model
| Input | Process | Output |
|----------|----------|----------|
| number | Check if number > 50 | Message "Yes" or "No"

#### 💻 Pseudocode
```text
START 
    Read number
    If number > 50 
        Display "Yes"
    Else
        Display "No"
    End If
END
```
#### 🧮 Flow Chart

![Flowchart for question 1](Q2.png)

### Question 3
| Input | Process | Output |
|----------|----------|----------|
| mark | Check if number >= 40 | Message "Pass" or "Fail" 
#### 📊 IPO Model
| Input | Process | Output |
|----------|----------|----------|
| number | Check if number > 50 | Message "Yes" or "No"

#### 💻 Pseudocode
```text
START 
    Read mark
    If mark >= 40
        Display "Pass"
    Else
        Display "Failed"
    End if
END
```
#### 🧮 Flow Chart
```mermaid
flowchart TD
    A([START]) --> B[/Read mark/]
    B --> C{mark >= 40 ?}
    C --> |Yes| D[/Display "Pass"/]
    C --> |No| E[/Display "Failed"/]
    D --> F([END])
    E --> F
    
```



### Question 4
| Input | Process | Output |
|----------|----------|----------|
| - dice1_value <br> -dice2_value | Check whose dice value greater| Message of "Player 1 Win" or "Player 2 Win" or "Tie"

#### 💻 Pseudocode
```text
START 
    Read dice1_value,dice2_value
    If dice1_value > dice2_value
        Display "Player 1 Win"
    Else if dice2_value > dice1_value
        Display "Player 2 Win"
    Else
        Display "Tie"
    End If
END
```
#### 🧮 Flow Chart
```mermaid
flowchart TD
    A([START]) --> B[/Read dice1_value,<br> dice2_value/]
    B --> C{dice1_value > dice2_value?}
    C --> |Yes| D[/Display "Player 1 Win"/]
    C --> |No| E{dice2_value > dice1_value}
    D --> H([END])
    E --> |Yes| F[/PDisplay "Player 2 Win" /]
    E --> |No| G[/Display "Tie"/]
    F --> H
    G --> H

    
```

### Question 5
#### 📊 IPO Model
| Input | Process | Output |
|----------|----------|----------|
| - length <br> - width | Calculate the perimeter based on length and width | perimeter


#### 💻 Pseudocode
```text
START 
    Read length,width
    perimeter = 2*(length + width)
    Display perimeter
END
```
#### 🧮 Flow Chart
```mermaid
flowchart TD
    A([START]) --> B[/Read length,width/]
    B --> C[perimeter = 2 * length + <br> 2 * width]
    C --> D[/Display perimeter/]
    D --> E([END])
    
```

### Question 6
#### 📊 IPO Model
| Input | Process | Output |
|----------|----------|----------|
| - | Find minimum of 10 random numbers| minimum of 10 random numbers


#### 💻 Pseudocode
```text
START 
    Initialize empty list numbers

    For i = 1 To 10 
        Generate random_number
        numbers[i] = random_number
    End for

    min = numbers[0]

    For each number In numbers Do
        If number < min 
            min = number

    Display the minimum of 10 random number
END
```
#### 🧮 Flow Chart
```mermaid
flowchart TD
    A([START]) --> B[Generate 10 <br> random number]
    B --> C[Find the minimum of 10 <br> random number]
    C --> D[/Display the minimum of 10 <br> random number/]
    D --> E([END])
    
```
### Question 7
#### 📊 IPO Model
| Input | Process | Output |
|----------|----------|----------|
| -  | - Generate 10 random numbers <br> - Check if each of number is odd then add to num_odd <br> - Check if each of number is even then add to num_even | - num_odd <br> - num_even


#### 💻 Pseudocode
```text
START 
    Initialize empty list numbers

    For i = 1 To 10 
        Generate random_number
        numbers[i] = random_number
    End for

    For each number in numbers 
        If number <= 100 and number >= 10
            If number % 2 == 0
                num_even = num_even + 1
            Else
                num_odd = num_odd + 1

    Display num_even, num_odd
END
```
#### 🧮 Flow Chart
```mermaid
flowchart TD
    A([START]) --> B[Generate 10 <br> random numbers]
    B --> C{All number processed?}
    C --> |No| D{number <= 100 and number >= 10 ?}
    D --> |Yes| E{number % 2 == 0?}
    E --> |Yes| F[num_even = num_even + 1]
    E --> |No| G[num_odd = num_odd + 1]
    F --> J[Proceed to next number]
    G --> J
    J --> C
    C --> |Yes| H[/Display num_even, <br> num_odd/]
    D --> |No| C
    H --> I([END])
    
    
```

### Question 8
#### 📊 IPO Model
| Input | Process | Output |
|----------|----------|----------|
| sentence | Count the number of alphabet U and M in sentence| - num_u <br> - num_m


#### 💻 Pseudocode
```text
START 
    Read sentence
    For each alphabet in sentence
        If alphabet == "U"
            num_u += 1
        Else if alphabet == "M"
            num_m += 1
        End If
    End For
    Display num_u,num_m
END
```
#### 🧮 Flow Chart
```mermaid
flowchart TD
    A([START]) --> B[/Read sentence/]
    B --> C{All alphabet processed?}
    C --> |Yes| D[/Display num_u, num_m/]
    C --> |No| E{alphabet == 'U' ?}
    E --> |Yes| F[num_u += 1]
    F --> C
    E --> |No| G{alphabet == 'M' ?}
    G --> |Yes| H[num_m += 1]
    H --> I[Proceed to next word]
    F --> I
    G --> |No| I
    I --> C
    D --> J([END])
    

```
### Question 9
#### 📊 IPO Model
| Input | Process | Output |
|----------|----------|----------|
| keyword | Count the frequency of keyword in web page| frequency


#### 💻 Pseudocode
```text
START 
    Read keyword
    For each word in keyword
        If word == keyword
            frequency += 1
        End if
    End For
    Display frequency
END
```
#### 🧮 Flow Chart
```mermaid
flowchart TD
    A([START]) --> B[/Read keyword/]
    B --> C{All word done searching?}
    C --> |Yes| D[/Display frequency/]
    C --> |No| E{word == keyword?}
    E --> |Yes| F[frequency += 1]
    E --> |No| I[Proceed to next word]
    F --> I
    I --> C
    D --> H([END])
    
```

### Question 10
#### 📊 IPO Model
| Input | Process | Output |
|----------|----------|----------|
| - |- Generate 100 student's gender <br> - Count the number of female student| num_female


#### 💻 Pseudocode
```text
START
    Initialize empty list genders
    For i = 1 To 100 
        Generate random_char 'M' or 'F'
        genders[i] = random_char
    End for

    Generate 100 student's gender
    For each gender in genders
        If gender == "F"
            num_female += 1
        End If
    End For
    Display num_female
END
```
#### 🧮 Flow Chart
```mermaid
flowchart TD
    A([START]) --> B[Generate 100 <br> student gender]
    B --> C{All student done processing?}
    C --> |No| D{gender == 'F'?}
    D --> |Yes| E[num_female += 1]
    D --> |No| G[Proceed to next student]
    E --> G
    G --> C
    C --> |Yes| F[/Display num_female/]
    F --> H([END])
```

### Question 11
#### 📊 IPO Model
| Input | Process | Output |
|----------|----------|----------|
| - |- Generate 5 random number <br> - Store them in a list <br> - Sort the list in descending order| 5 random number in descending order


#### 💻 Pseudocode
```text
START 
    Initialize empty list numbers

    For i = 0 To 4
        Generate random_number
        Set numbers[i] = random_number
    End for

    temp = 0

    For i = 0 To 4
        For j = 0 To (4-i-1) 
            If numbers[j] < numbers[j+1]
                temp = numbers[j]
                numbers[j] = numbers[j+1]
                numbers[j+1] = temp
            End If
        End For
    End For 

    Display numbers list
END
```
#### 🧮 Flow Chart
```mermaid
flowchart TD
    A([START]) --> B[Generate 5 <br> random numbers]
    B --> C[Store numbers in list]
    C --> D[Sort list in descending order]
    D --> E[/Display sorted list/]
    E --> F([END])
```

### Question 12
#### 📊 IPO Model
| Input | Process | Output |
|----------|----------|----------|
| guess |- Generate a random number - Check if guess same with random number| Message "Correct" or "Wrong"


#### 💻 Pseudocode
```text
START 
    Generate random number
    Read guess 
    If guess == random number
        Display "Correct"
    Else
        Display "Wrong"
END
```
#### 🧮 Flow Chart
```mermaid
flowchart TD
    A([START]) --> B[Generate  random numbers]
    B --> C[/Read guess from user/]
    C --> D{ guess == random number?}
    D --> |Yes| E[/Display 'Correct'/]
    D --> |No| F[/Display 'Wrong'/]
    E --> G([END])
    F --> G
```

