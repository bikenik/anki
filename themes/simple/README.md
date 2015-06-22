# Anki theme: Simple
## Anki complex theme for programming snippets

A simple question/answer card. If you need more flexibility the [complex theme](../complex/README.md) may be more appropriate.

## Fields:

1. **Title**
  - The main question, statement or fact
2. **Syntax** – *(optional)*
  - The main `syntax` we're learning
3. **Syntax code** - *(optional)*
  - The actual function or symbol, i.e. `len()`
  - This will be wrapped in `<code>`
4. **Sample code image** - *(optional)*
  - Upload a snapshot of the code we're learning
5. **Key point (code)**
  - What's the main takeaway from this flashcard? (Small statement or snippet of code)
  - This will be wrapped in `<pre><code>`
  - You can colour code using:
    - `<span>` for blue,
    - `<strong>` or `<b>` for pink,
    - `<em>` or `<i>` for purple,
    - `<small>` for comments
6. **Key point image** – *optional*
  - Complementary image
7. **Key point notes**
  - A short explanation of what we're trying to learn
  - For any key functions or symbols, wrap in `<code>`
8. **Other notes** – *optional*
  - A more in-depth explanation of what we're trying to learn, or any supplementary notes for either `Key points` or `Puzzle`


## Cards

There's 3 cards here:

### 1. What's the answer?

A simple question/answer. From the `syntax`, `syntax code` and the `title`, guess the answer. Must have at least `Key point (code)` or `Key point notes` filled.

### 2. What does this symbol do?

A slight variation on the 1st card. From the `syntax` and `syntax` code, guess the function or symbol's uses. Must have at least `Key point (code)` or `Key point notes` filled.

### 3. Puzzle question (optional)

Here we can get creative. As we don't have `syntax` or `syntax code`, create a puzzle question which forces you to guess how to solve a specific problem and with what function you'd need to do so. Must have at least `Puzzle` and `Puzzle answer notes` filled — often `Sample code image` and `Key points (code)` give enough examples to know if you've solved the puzzle properly.

This template is a little complex so may have to be revisited, it assumes the following:

1. If the `Puzzle hint (code)` is filled out, don't show the `Sample code image` but add it as a reference below.
2. If `Puzzle hint (code)` is not filled out, it assumes that the `Sample code image` is the answer so displays it above any `Puzzle answer notes`.


## Notes

1. [Style fields, inline code and code blocks](../../README.md)
2. Fields marked **optional** can be left blank and the template will ignore them. If all fields are used, 3 cards will be generated.
3. You can reference fields within fields. For instance, `{{Syntax code}}` or `{{Key point (code)}}` - this will pick up all the HTML from those fields. If you want the fancy code styles, you'll need to select *Edit HTML* in Wysiwig and wrap in `<code>`, it'll be rendered as an inline code block.