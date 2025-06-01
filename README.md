````markdown
# Truncate a String

A simple utility function to truncate a string to a specified length. If the string exceeds the given length, it will be shortened and appended with `...`. If the string length is equal to or less than the specified limit, it will be returned unchanged.

## Features

- Truncates strings longer than the specified length.
- Appends `...` to indicate truncation.
- Returns strings unchanged if they are shorter or equal in length to the limit.

## Usage

### Function Signature

```js
truncateString(str, num)
```

* `str` — The input string to truncate.
* `num` — The maximum allowed length of the string before truncation.

### Example

```js
truncateString("Hello, world!", 5);  // Returns: "Hello..."
truncateString("Short", 10);          // Returns: "Short"
truncateString("Exact", 5);           // Returns: "Exact"
```

## Installation

No installation required. This is a simple function that can be copied into any JavaScript project.

## How It Works

* If the input string length is greater than `num`, the function slices the string from the start to the `num`th character and appends `"..."`.
* If the string length is less than or equal to `num`, it returns the original string without changes.

## Testing

You can test the function by running the following examples:

```js
console.log(truncateString("Hello, world!", 5));  // Output: "Hello..."
console.log(truncateString("Short", 10));         // Output: "Short"
console.log(truncateString("Exact", 5));          // Output: "Exact"
```

## License

This project is open source and free to use.
