# Working With Custom Attributes

### What Custom Attributes Are

Custom Attributes let you attach **extra information** to elements in your email or landing page—such as links, buttons, or images—without changing what people see in the editor.\
Think of them as **invisible labels or instructions** that your company or platform uses later when the message is sent, tracked, or analyzed.

For example, you could:

* Tag links that should _not_ be tracked for analytics.
* Add accessibility details (so screen readers can describe links or images properly).
* Pass internal data for personalization or reporting.
* Indicate which version of a block belongs to an A/B test.

### Why They’re Useful

Adding Custom Attributes helps your company’s tools work better behind the scenes:

* **Analytics & segmentation:** identify clicks that belong to a specific campaign or audience.
* **Accessibility:** improve how assistive technologies read your content (e.g., via `aria-label`).
* **Styling & customization:** add CSS classes that designers or developers can target.
* **Compliance & privacy:** mark elements that shouldn’t be tracked or stored.
* **Localization:** guide translation systems by marking which content should or shouldn’t be translated.

In short, Custom Attributes give your content **intelligence**—making every email or page smarter and easier to process.

### Where You’ll Find Custom Attributes in the Editor

Depending on what you’re editing, you’ll find Custom Attributes in slightly different places:

* **Buttons and Images:** in the **right-hand sidebar**, under the **Attributes** section.
* **Links inside text:** when you add or edit a link, look for the **Attributes** area in the link dialog.
* **Social, Menu, and Icon blocks:** open the block’s settings and look for the **Attributes** panel.

### How to Add a Custom Attribute

1. **Select the content** (e.g., a button, image, or link) you want to tag.
2. In the **Attributes** section:
   * Choose an attribute name from the list provided (like `data-segment` or `aria-label`), **or** create a new one if allowed.
   * Enter or pick a value.
3. **Save or close** the dialog.\
   The attribute is now part of your element—visible to your company’s systems, not your audience.

Example:

```html
<a href="https://example.com" data-segment="travel" aria-label="Read more about travel">Read more</a>
```

### Examples of Attributes You Might See

| Attribute name | What it does                   | Example value           | Used for                    |
| -------------- | ------------------------------ | ----------------------- | --------------------------- |
| `data-segment` | Marks a segment or campaign    | `travel`, `luxury`      | Reporting / personalization |
| `aria-label`   | Adds an accessible description | `Follow us on LinkedIn` | Accessibility               |
| `class`        | Assigns a CSS class            | `untracked`             | Styling / tracking control  |
| `data-test-id` | Identifies elements in tests   | `hero-title`            | A/B or QA testing           |

### Tips for Using Them Wisely

* Only use attributes you understand—check your team’s internal documentation if unsure.
* For accessibility, use `aria-` attributes thoughtfully to describe content, not repeat it.
* If you’re adding a tracking or testing tag, double-check spelling: your analytics may depend on it!
* Don’t over-tag everything—focus on attributes your organization actively uses.

### When You Can’t Edit Custom Attributes

Some attributes may be **locked** by your organization’s admin or developer team.\
You’ll still see them, but you won’t be able to modify or remove them—this ensures consistency and compliance.

### Summary

| Feature                 | What It Does                                                           | Where To Find It       |
| ----------------------- | ---------------------------------------------------------------------- | ---------------------- |
| Add metadata to content | Append invisible instructions for analytics, styling, or accessibility | Sidebar or link dialog |
| Predefined attributes   | Choose from a curated list                                             | Sidebar                |
| Custom attributes       | Type your own name & value                                             | If allowed             |
| Accessibility support   | Add `aria-*` or `role` info                                            | Any supported block    |

#### Why It Matters

Using Custom Attributes ensures that your company’s emails and landing pages are **data-ready, accessible, and compliant**—without adding complexity for you.\
They make your design not only beautiful but also meaningful to the systems that power your campaigns.
