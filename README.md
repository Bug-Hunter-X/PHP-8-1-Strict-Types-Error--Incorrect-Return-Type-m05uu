# PHP 8.1 Strict Types Error: Incorrect Return Type

This example demonstrates a common error encountered when using strict types in PHP 8.1 and above.  The function `foo` is declared to return an integer (`int`), but in certain cases, it might return a different type. This will cause a fatal error.

The `bug.php` file contains the erroneous code, and `bugSolution.php` provides a corrected version.

## How to reproduce

1. Save the code from `bug.php`.
2. Execute the script using a PHP 8.1 or higher interpreter.  
3. You will observe a fatal error indicating type mismatch.

## Solution

The solution involves carefully checking function logic to ensure it always returns a value of the declared type.  If that is not possible, change the return type hint or handle potential exceptions which may cause unexpected return types.  The correct version can be found in `bugSolution.php`