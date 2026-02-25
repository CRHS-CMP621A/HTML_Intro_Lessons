# Intro to HTML — 5-Day Unit Plan

**Grade 12 Computer Science**

A five-day unit plan covering the fundamentals of web markup — from document structure to forms — preparing students for CSS.

- **Duration:** 5 Days
- **Level:** Grade 12
- **Prerequisites:** None
- **Next Unit:** Intro to CSS

---

## Daily Overview

| Day | Topic            | Focus                           |
| --- | ---------------- | ------------------------------- |
| 01  | Web Foundations  | Document Structure              |
| 02  | Text & Semantics | Block vs. Inline                |
| 03  | Links & Media    | Hyperlinks, Images, Video/Audio |
| 04  | Lists & Tables   | Organizing Information          |
| 05  | Forms & Project  | Putting It All Together         |

---

## Day 1: Web Foundations & Document Structure

Students learn what HTML is, how browsers interpret markup, and how to write their first valid HTML document from scratch.

### Learning Objectives

1. Explain what HTML is and its role in the web stack (HTML, CSS, JS)
2. Describe how a browser parses and renders an HTML document
3. Identify the anatomy of an HTML element: opening tag, content, closing tag
4. Distinguish between elements, tags, and attributes
5. Write a syntactically valid HTML5 document from memory
6. Use a code editor and preview a page in a browser

### Lesson Schedule (75 min)

**Warm-Up — 5 min**

- Ask students: "What actually happens when you type a URL and press Enter?"
- Collect 4–5 responses on the board. Don't correct yet — revisit at the end.

**Instruction — 20 min**

- Introduce HTML as a markup language. Distinguish markup from programming.
- Show the browser developer tools "Elements" tab on a real website. Webpage [Superhero Profile](https://kasslent.github.io/superhero-profiles/)
- Explain the request/response cycle at a high level.  Video [The Internet: HTTP & HTML (Code.org)](https://www.youtube.com/watch?v=kBXQZMmiA4s)

**Instruction — 15 min**

- Anatomy of HTML: elements, tags, attributes.  Web Resource: [Tags vs Elements vs Attributes](https://www.geeksforgeeks.org/html/tags-vs-elements-vs-attributes-in-html/)
- Show tag = opening + closing.  
- Introduce self-closing tags. **Create a tags.html file in L1, add tags**
- Walk through the HTML5 boilerplate live on the projector: `<!DOCTYPE>`, `<html>`, `<head>`, `<meta charset>`, `<title>`, `<body>`. **Show students how to open/preview L1_reference_code.html**

**Guided Practice — 25 min**

- Students open VS Code (or chosen editor). 
- Create a **new_page.html** file in L1 folder.
- Instructor types the boilerplate live; students follow along.
- Students add their name in the title, write one heading, and one paragraph.
- Open in browser — first page!

**Wrap-Up — 10 min**

- Return to warm-up responses. Correct misconceptions.
- Extra: Copy and paste into W3 Validator
- Review the Learning Objectives for this Lesson.
- Students write an exit ticket: draw and label an HTML element from memory.

### Key Concepts & Vocabulary

- **HTML:** HyperText Markup Language — describes structure, not style
- **`<!DOCTYPE>`:** Declaration that tells the browser this is HTML5
- **Element:** The full unit: opening tag + content + closing tag
- **Tag:** The angle-bracket markers, e.g. `<p>`
- **Attribute:** Extra info inside a tag: `name="value"`
- **`<head>`:** Metadata container — not displayed on the page
- **`<body>`:** Everything visible to the user lives here
- **Nesting:** Placing elements inside other elements

### Reference Code: HTML5 Boilerplate

```html
<!-- Every HTML file starts here -->
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Page Title</title>
  </head>
  <body>
    <!-- Visible content goes here -->
    <h1>Hello, World!</h1>
    <p>My first HTML page.</p>
  </body>
</html>
```

### Teacher Notes & Differentiation

#### 💡 Teacher Tip

Use browser dev tools as your most powerful teaching prop. Right-click any website → Inspect → show how every visible element maps to HTML. Students are instantly hooked when they see real, familiar sites deconstructed.

#### Common Misconceptions to Address

- **"HTML is a programming language"** — Clarify it's a markup/structure language; it describes content, not logic.
- **Forgetting to close tags** — Emphasize that most tags come in pairs. Show how a missing `</body>` can break layout.
- **The doctype is a tag** — It's a declaration, not an element. It has no closing tag.

#### Extension for Advanced Students

- Research the history of HTML versions (HTML 1.0 to HTML5). What changed?
- Use the W3C validator (validator.w3.org) to check their boilerplate and interpret the output.

#### Support for Struggling Students

- Provide a printed boilerplate template they can annotate by hand before typing.
- Pair them with a stronger student for the guided practice phase.

---

## Day 2: Text, Semantics & Block vs. Inline

Students learn to work with text content using the correct semantic elements, and develop an understanding of the block vs. inline display model that underpins CSS layout.

### Learning Objectives

1. Use heading elements `<h1>`–`<h6>` with correct hierarchy
2. Write paragraphs, line breaks, and horizontal rules
3. Apply inline text elements: `<strong>`, `<em>`, `<span>`, `<mark>`, `<code>`
4. Explain semantic HTML: choosing elements based on meaning, not appearance
5. Distinguish block elements from inline elements and predict their behavior
6. Use HTML comments to annotate code

### Lesson Schedule (75 min)

**Warm-Up — 5 min**

- Show two HTML snippets: one using `<b>` everywhere, one using `<strong>`, `<em>`, and headings.
- Ask: "Which is better? Why might the second matter to a screen reader?"

**Instruction — 20 min**

- Walk through headings (H1–H6) as a document outline, not a size selector.
- Introduce paragraphs and `<br>`.
- Cover the semantic principle: HTML = meaning, CSS = appearance.
- Show a screen reader demo (NVDA or VoiceOver) on a well-structured vs. poorly structured page.

**Instruction — 15 min**

- Inline text elements: `<strong>` (importance) vs `<b>` (visual bold), `<em>` (stress emphasis) vs `<i>` (italic style).
- Introduce `<span>` as the generic inline container, `<mark>` for highlighted text, `<code>` for inline code snippets.
- **Block vs. inline:** Block elements stack vertically and take full width; inline elements flow within text.

**Guided Practice — 25 min**

- Students recreate a formatted article about a topic of their choice.
- Requirements: one H1, two H2s, at least three paragraphs, one use each of `<strong>`, `<em>`, and `<mark>`.

**Wrap-Up — 10 min**

- Pair discussion: "Could a search engine understand your page better because of how you used headings?"
- Collect exit ticket: name one block element and one inline element with a sentence explaining the difference.

### Key Concepts & Vocabulary

- **Semantic HTML:** Using elements that describe meaning, not just visual style
- **Block element:** Starts on a new line, stretches full width: `<p>`, `<h1>`
- **Inline element:** Flows within text: `<strong>`, `<em>`, `<span>`
- **`<strong>`:** Semantic importance — rendered bold, meaningful to screen readers
- **`<em>`:** Stress emphasis — rendered italic, meaningful to screen readers
- **`<span>`:** Generic inline container; no semantic meaning on its own
- **Accessibility:** Designing so screen readers and assistive tools work correctly
- **HTML comment:** `<!-- ... -->` — ignored by browser, useful for notes

### Reference Code: Text & Semantic Elements

```html
<h1>Article Title (H1 — only one per page)</h1>
<h2>Section Heading</h2>

<p>
  A regular paragraph of text. HTML won't respect your line breaks — use <br />
  for that.
</p>

<p>
  This is <strong>important</strong> and this is <em>emphasized</em> text. You
  can also <mark>highlight</mark> text, or show <code>inline code</code>.
</p>

<!-- span has no default meaning - style with CSS later -->
<p>Price: <span>$9.99</span></p>
```

### Teacher Notes & Differentiation

#### 💡 Teacher Tip

The block vs. inline distinction is one of the most important conceptual foundations for CSS layout. Spending 5 extra minutes here with a visual diagram (draw boxes stacking vs. words flowing inline) will save significant confusion in the CSS unit. Return to this concept every time you introduce a new element.

#### Semantic HTML — Why It Matters (Talking Points)

- **Accessibility:** Screen readers use heading hierarchy to help visually impaired users navigate a page. Using H3 because "it looks like the right size" is harmful.
- **SEO:** Search engines weight H1 content more heavily. A well-structured page ranks better.
- **Maintainability:** Semantic code is easier to read and style. When CSS says "style all h2 elements," it only works if H2s are actually H2s.

#### Common Errors to Watch For

- Skipping heading levels (jumping from H1 to H4) — treat headings like an outline, not a size tool.
- Using `<br>` to add spacing between paragraphs — this should be done with CSS margin later.
- Nesting a block element inside an inline element (e.g., `<span><p>...</p></span>`) — invalid HTML.

---

## Day 3: Links, Images & Media

Students learn to connect pages with hyperlinks, embed images with accessible alt text, and get a first look at audio and video elements — the features that make the web truly "hyper."

### Learning Objectives

1. Create hyperlinks using `<a href>` and explain what href stands for
2. Distinguish absolute URLs from relative file paths
3. Use `target="_blank"` and explain its security implications
4. Embed images using `<img src alt>`
5. Write meaningful alt text that describes an image's purpose
6. Organize project files in a folder structure (assets/images)
7. Embed a video or audio element with basic controls

### Lesson Schedule (75 min)

**Warm-Up — 5 min**

- Show the class a webpage with a broken image icon and an empty `alt` attribute.
- Ask: "Who is affected when this image fails to load? Who else might always see this?"

**Instruction — 20 min**

- Hyperlinks: anatomy of `<a href="...">`.
- Absolute vs. relative paths with a folder diagram on the board.
- Demo: linking to Google (absolute), then to another local HTML file (relative).
- Introduce `target="_blank"` — and the `rel="noopener noreferrer"` security convention.

**Instruction — 15 min**

- Images: `<img>` is a self-closing (void) element.
- The `src` and `alt` attributes.
- How to write good alt text: describe function, not just appearance.
- Decorative images use `alt=""`.
- Brief intro to `<video>` and `<audio>` with `controls` attribute.

**Guided Practice — 25 min**

- Students set up a two-page mini-site: `index.html` and `about.html`, with an images/ subfolder.
- They link the pages to each other, add a navigation link to an external site, and embed at least two images with proper alt text.

**Wrap-Up — 10 min**

- Peer review: swap computers. Partner checks that images have alt text and links work.
- Discuss: "What makes a bad alt text?"
- Exit ticket: write alt text for a photo of a dog jumping to catch a frisbee in a park.

### Key Concepts & Vocabulary

- **Hyperlink:** A clickable reference to another resource or page
- **href:** Hypertext Reference — the URL the link points to
- **Absolute URL:** Full web address: `https://example.com/page.html`
- **Relative path:** Path relative to current file: `../images/dog.jpg`
- **Void element:** Self-closing tag with no children: `<img>`, `<br>`
- **alt attribute:** Alternative text for images — read by screen readers, shown if image fails
- **src:** Source — the file path or URL of a media resource
- **File structure:** Organizing HTML, CSS, and assets into logical folders

### Reference Code: Links, Images & Media

```html
<!-- Absolute link (external site) -->
<a href="https://www.wikipedia.org" target="_blank" rel="noopener noreferrer">
  Visit Wikipedia
</a>

<!-- Relative link (same project) -->
<a href="about.html">About Me</a>

<!-- Image with descriptive alt text -->
<img
  src="images/profile.jpg"
  alt="Student smiling at their laptop"
  width="300"
/>

<!-- Video with browser controls -->
<video src="clip.mp4" controls width="640">
  Your browser doesn't support video.
</video>
```

### Teacher Notes & Differentiation

#### 💡 Teacher Tip

The relative path lesson trips up many students. Draw the folder structure on the board as a tree diagram, then walk through 2–3 path examples physically: "We're in index.html. To get to images/logo.png, we go INTO the images folder." Use dot-dot-slash notation visually as "going up" one level.

#### Suggested Folder Structure for Student Projects

```
my-website/
├── index.html
├── about.html
└── images/
```

#### Security Note on target="\_blank"

- Opening a new tab gives the linked page access to your page via `window.opener`.
- Adding `rel="noopener noreferrer"` prevents this — a good professional habit to introduce early.

#### Alt Text Quality Rubric (for Peer Review)

- **Poor:** `alt="image"` or `alt="photo"` — says nothing
- **Okay:** `alt="dog"` — minimal but passes validation
- **Good:** `alt="Golden retriever catching a frisbee in a sunny park"` — describes context
- **Decorative:** `alt=""` — correct for purely decorative images (screen reader skips it)

---

## Day 4: Lists & Tables

Students learn to organize information using ordered and unordered lists, and to represent structured data using HTML tables — while developing a critical eye for when each is the right tool.

### Learning Objectives

1. Create ordered `<ol>` and unordered `<ul>` lists with `<li>` items
2. Build nested lists (a list inside a list item)
3. Build a complete HTML table with `<table>`, `<tr>`, `<th>`, and `<td>`
4. Use `<thead>`, `<tbody>`, and `<tfoot>` for table structure
5. Apply `colspan` and `rowspan` attributes
6. Explain when to use a table (tabular data) versus when NOT to (page layout)

### Lesson Schedule (75 min)

**Warm-Up — 5 min**

- Show a 90s-era website that used tables for layout (archive.org has examples).
- Ask: "What's wrong with this approach?" Collect guesses — revisit after instruction.

**Instruction — 15 min**

- Unordered lists: no sequence implied (navigation menus, ingredient lists).
- Ordered lists: sequence matters (step-by-step instructions, rankings).
- Demo nested lists: homework checklist with sub-tasks.
- Common mistake: putting anything other than `<li>` directly inside `<ul>`/`<ol>`.

**Instruction — 20 min**

- Tables: start with a simple 3-column schedule.
- Introduce `<table>` → `<tr>` → `<th>`/`<td>`.
- Add semantic grouping: `<thead>`, `<tbody>`.
- Demonstrate `colspan="2"` to merge two columns.
- **Critical rule:** Tables are for tabular data, NOT page layout.

**Guided Practice — 25 min**

- **List challenge:** Create a nested shopping list with 3 categories, each with 3 items.
- **Table challenge:** Build a class schedule table with days as columns and periods as rows. Add a merged header cell for "Weekend."

**Wrap-Up — 10 min**

- Return to warm-up screenshot. Students now explain the problem.
- Exit ticket: "Give one example of data that belongs in a table, and one that does not."

### Key Concepts & Vocabulary

- **`<ul>`:** Unordered list — bullet points, no sequence implied
- **`<ol>`:** Ordered list — numbered, sequence matters
- **`<li>`:** List item — must be a direct child of `<ul>` or `<ol>`
- **`<table>`:** Container for tabular data with rows and columns
- **`<tr>`:** Table row
- **`<th>`:** Table header cell — bold and centered by default
- **`<td>`:** Table data cell
- **colspan:** Merges a cell across multiple columns

### Reference Code: Lists & Tables

```html
<!-- Nested unordered list -->
<ul>
  <li>
    Fruit
    <ul>
      <li>Apples</li>
      <li>Bananas</li>
    </ul>
  </li>
</ul>

<!-- Structured table with merged header -->
<table>
  <thead>
    <tr>
      <th>Name</th>
      <th colspan="2">Scores</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Alex</td>
      <td>85</td>
      <td>92</td>
    </tr>
  </tbody>
</table>
```

### Teacher Notes & Differentiation

#### 💡 Teacher Tip

Tables are highly visual — build them row by row on the projector. After each `<tr>`, refresh the browser so students see the table grow. This makes the row/cell relationship concrete. Having students draw the expected table grid on paper before coding it dramatically reduces errors.

#### The "Tables for Layout" Anti-Pattern (Historical Context)

- Before CSS was widely supported (~1999–2005), developers used invisible tables to position content in columns. This was a workaround, not a feature.
- Today, tables for layout are an accessibility violation (screen readers announce table structure) and are never used in professional code.
- This history makes for a great 5-minute discussion about how standards evolve.

#### Common Table Errors

- Mismatched cell counts per row — every row must have the same number of cells (accounting for colspan).
- Forgetting `</tr>` closing tags — causes all remaining rows to collapse.
- Using `<td>` for headers instead of `<th>` — loses semantic meaning and accessibility.

---

## Day 5: Forms & Mini-Project

Students learn to build interactive HTML forms, then apply everything from the week to create a complete multi-element webpage — their launchpad for the CSS unit.

### Learning Objectives

1. Create a form using `<form>` with a meaningful `action` attribute
2. Add labeled inputs: text, email, password, number, date
3. Use `<label>` correctly with the `for`/`id` connection
4. Implement checkbox, radio button, and select dropdown inputs
5. Add a `<textarea>` and a submit button
6. Produce a complete HTML page combining all elements from the unit
7. Articulate why CSS is the natural next step

### Lesson Schedule (75 min)

**Warm-Up — 5 min**

- Show a sign-up form on screen.
- Ask: "What HTML elements do you think are used to build this? Write your guesses."
- Students will be surprised how many they already recognize.

**Instruction — 20 min**

- The `<form>` element and the `action` attribute (where data goes on submit).
- Introduce `<label>` and the critical `for`/`id` link — clicking a label focuses its input.
- Common input types: text, email, password, number, checkbox, radio.
- The `name` attribute — how form data is identified.
- `<select>` + `<option>` dropdowns.
- `<textarea>` for multi-line text.
- Submit button with `<button type="submit">`.

**Mini-Project — 40 min**

**Personal Profile Page.** Students build a complete page with:

- A proper HTML5 boilerplate
- A heading with their name
- A short bio paragraph using `<strong>` and `<em>`
- A profile image with alt text
- A navigation bar with links (home, about, contact) using a `<ul>`
- A table showing their weekly schedule
- A contact form with name, email, message textarea, and submit

This file becomes their starting point for CSS styling next week.

**Wrap-Up — 10 min**

- Gallery walk — students leave their browser open and walk around to see each other's pages.
- Discussion: "Every page looks plain and unstyled. What would you change if you could? That's exactly what CSS does."
- Preview the CSS unit.

### Key Concepts & Vocabulary

- **`<form>`:** Container that groups inputs and sends data on submit
- **action:** URL that receives the form data when submitted
- **`<label>`:** Describes an input; `for` attr links it by `id`
- **name attr:** Key used to identify the input's value when form is submitted
- **type attr:** Defines input behavior: text, email, password, checkbox, radio…
- **`<select>`:** Dropdown menu; populated with `<option>` elements
- **`<textarea>`:** Multi-line text input — rows/cols set initial size
- **required:** HTML attribute that prevents submission if field is empty

### Reference Code: HTML Form

```html
<form action="/submit" method="post">
  <!-- Label links to input via matching for/id -->
  <label for="username">Name:</label>
  <input type="text" id="username" name="username" required />

  <label for="email">Email:</label>
  <input type="email" id="email" name="email" />

  <!-- Radio buttons share the same name -->
  <input type="radio" name="grade" id="g11" value="11" />
  <label for="g11">Grade 11</label>

  <!-- Dropdown -->
  <select name="subject">
    <option value="cs">Computer Science</option>
    <option value="math">Math</option>
  </select>

  <label for="msg">Message:</label>
  <textarea id="msg" name="msg" rows="4"></textarea>

  <button type="submit">Send</button>
</form>
```

### Teacher Notes & Differentiation

#### 💡 Teacher Tip

The gallery walk at the end is powerful pedagogy. When every student sees that raw HTML looks identical in style — plain browser defaults — the motivation to learn CSS is visceral and personal. "That's MY page and it looks boring" is more compelling than any amount of explanation.

#### Mini-Project Assessment Checklist

- ✓ Valid HTML5 boilerplate with correct doctype, head, and body
- ✓ Heading hierarchy used correctly (one H1, logical H2/H3 usage)
- ✓ At least one image with meaningful, non-empty alt text
- ✓ At least two working hyperlinks (one internal, one external)
- ✓ A list (ordered or unordered) used appropriately
- ✓ A table with `<thead>`, `<tbody>`, `<th>`, and `<td>`
- ✓ A form with at least four inputs, all properly labeled with `<label>`
- ✓ Code is consistently indented and readable

#### Bridging to CSS — Discussion Prompts

- "Your page is structured but unstyled. In CSS, you'll select elements by tag name, class, or ID to apply styles. Notice that your HTML already uses IDs on form inputs — those will become CSS hooks."
- "Every HTML element has a default browser style. CSS lets you override any of them — fonts, colors, spacing, layout, animations."
- "The block vs. inline distinction you learned today is the foundation of the CSS box model. You'll come back to it constantly."

---

## Unit Cheat Sheet

_Distribute to students on Day 1 — they add to it each day_

### Day 1 — Structure

```html
<!DOCTYPE html>
<html>
  <head>
    <title>…</title>
  </head>
  <body>
    <!-- visible content -->
  </body>
</html>
```

### Day 2 — Text

```html
<h1>
  –
  <h6>
    <p>
      <br />
      <strong>
        <em>
          <mark>
            <code>
              <span> <!-- block vs. inline --></span></code
            ></mark
          ></em
        ></strong
      >
    </p>
  </h6>
</h1>
```

### Day 3 — Links & Media

```html
<a href="url">Link</a>
<img src="…" alt="desc" />
<video src="…" controls></video>
```

### Day 4 — Lists & Tables

```html
<ul>
  <li>…</li>
</ul>
<ol>
  <li>…</li>
</ol>
<table>
  <tr>
    <th>H</th>
    <td>Data</td>
  </tr>
</table>
```

### Day 5 — Forms

```html
<form action="…">
  <label for="x">Label</label>
  <input type="text" id="x" name="x" />
  <select name="s">
    <option>…</option>
  </select>
  <textarea name="msg"></textarea>
  <button type="submit">Submit</button>
</form>
```

---

**End of Unit Plan**
