# Doc

# 📜 Quote Display with JavaScript

This project demonstrates a simple use of JavaScript to display a random motivational quote after a short delay. It's a great beginner-friendly exercise that helps you understand core JavaScript concepts like arrays, DOM manipulation, and timers.

---

## 🔧 How It Works

```
setTimeout(() => {
    const quotes = [
        "The best way to predict the future is to create it.",
        "Do what you can, with what you have, where you are.",
        "Success is not final, failure is not fatal: it is the courage to continue that counts.",
        "Believe you can and you're halfway there."
    ];

    const randomQuote = quotes[Math.floor(Math.random() * quotes.length)];
    quoteBox.innerText = randomQuote;
    quoteBox.style.display = "block";
    loading.style.display = "none";
}, 2000);
```

---

## 🧠 Line-by-Line Explanation

### `setTimeout(() => { ... }, 2000);`

- Waits **2 seconds** (2000 milliseconds), then runs the function inside.

### `const quotes = [ ... ];`

- Stores an array of motivational quote strings.

### `const randomQuote = quotes[Math.floor(Math.random() * quotes.length)];`

- Picks one quote at random:
    - `Math.random()` generates a number between 0 and 1.
    - Multiply by `quotes.length` to scale it to array size.
    - `Math.floor(...)` rounds it down to a valid index.

### `quoteBox.innerText = randomQuote;`

- Updates the HTML element with the chosen quote.

### `quoteBox.style.display = "block";`

- Makes the quote box visible.

### `loading.style.display = "none";`

- Hides the loading indicator.

---

## 🧪 How To Use

1. Make sure you have a `div` or `span` with the id `quoteBox` in your HTML.
2. Also have a `div` or `span` with the id `loading` to show a loading message.
3. Link this JavaScript code to your HTML file.

---

## 📁 Example HTML Structure

```
<div id="loading">Loading...</div>
<div id="quoteBox" style="display: none;"></div>
```

---

## 🏁 Result

After 2 seconds, the loading message disappears and a random quote is shown in the quote box.

---

## 📚 Perfect For Learning:

- JavaScript arrays
- Random selection
- setTimeout
- DOM manipulation
- Beginner projects

Happy coding! 🚀
