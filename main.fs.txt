// Define a function that calculates the factorial of a number
let rec factorial n =
    if n <= 1 then
        1
    else
        n * factorial (n - 1)

// Define a function that uses pattern matching to identify the day of the week
let dayOfWeek day =
    match day with
    | 1 -> "Monday"
    | 2 -> "Tuesday"
    | 3 -> "Wednesday"
    | 4 -> "Thursday"
    | 5 -> "Friday"
    | 6 -> "Saturday"
    | 7 -> "Sunday"
    | _ -> "Invalid day"

// Define a list of numbers and calculate their squares
let numbers = [1; 2; 3; 4; 5]
let squares = List.map (fun x -> x * x) numbers

// Print the factorial, day of the week, and squares
let () =
    printfn "Factorial of 5: %d" (factorial 5)
    printfn "Day 3 of the week: %s" (dayOfWeek 3)
    printfn "Squares of numbers: %A" squares
