# Bulma.sketch UI Kit

**Bulma.sketch** is a Sketch file (<https://www.sketchapp.com/>) for Bulma CSS Framework (<http://bulma.io>).

Bulma version : **v0.5.1**

## How is it used ?

## Basics

### Colors

**Bulma.sketch uses colors as Symbols for background and border colors. `Symbol > colors` contains initial colors (`$turquoise`, `$blue`, `$yellow`…) and derived colors (`$primary`, `$info`, `$warning`…)**

#### Initial colors

[Bulma ref](http://bulma.io/documentation/overview/variables/#initial-variables)

| Bulma variable | Symbol path |
|:--|:--|
|  `$black`   |   `Symbol > colors/black`  |
|  `$black-bis`   |   `Symbol > colors/black-bis`  |
|  `$black-ter`   |   `Symbol > colors/black-ter`  |
|  `$grey-darker`   |   `Symbol > colors/grey-darker`  |
|  `$grey-dark`   |   `Symbol > colors/grey-dark`  |
|  `$grey`   |   `Symbol > colors/grey`  |
|  `$grey-light`   |   `Symbol > colors/grey-light`  |
|  `$grey-lighter`   |   `Symbol > colors/grey-lighter`  |
|  `$white-ter`   |   `Symbol > colors/white-ter`  |
|  `$white-bis`   |   `Symbol > colors/white-bis`  |
|  `$white`   |   `Symbol > colors/white`  |
|  `$orange`   |   `Symbol > colors/orange`  |
|  `$yellow`   |   `Symbol > colors/yellow`  |
|  `$green`   |   `Symbol > colors/green`  |
|  `$turquoise`   |   `Symbol > colors/turquoise`  |
|  `$blue`   |   `Symbol > colors/blue`  |
|  `$purple`   |   `Symbol > colors/purple`  |
|  `$red`   |   `Symbol > colors/red`  |

#### Derived colors 

[Bulma ref](http://bulma.io/documentation/overview/variables/#derived-variables)

| Bulma variable | Symbol path |
|:--|:--|
| `$primary` | `Symbol > colors/primary` |
| `$info` | `Symbol > colors/info` |
| `$success` | `Symbol > colors/success` |
| `$warning` | `Symbol > colors/warning` |
| `$danger` | `Symbol > colors/danger` |
| `$light` | `Symbol > colors/light` |
| `$dark` | `Symbol > colors/dark` |


### Typography helpers

[Bulma ref.](http://bulma.io/documentation/modifiers/typography-helpers/)

**For better usage, some typography variants have been made available as Symbols.**

You have all sizes (`is-size-1` to `is-size-7`), all primary colors (`has-text-black` to `has-text-danger`), all alignments (~~lawful good to chaotic evil~~ `has-text-left`, `has-text-centered` and `has-text-right`).

All these variants are available through `Symbol > typography`.

E.g.: for a text with Bulma classes `.has-text-danger.is-size-3.has-text-centered`, the Symbol to insert is found at `Symbol > typography/has-text-danger/is-size-3 has-text-c`

#### Remarks :

`is-lowercase` and `is-uppercase` could be added, but it will add mostly unnecessary Symbols to an already heavy Symbol collection. `is-capitalized` wouldn't be possible.

No responsive variants have been added, it wouldn't be possible due to Sketch limitations.

---

## Form

### General

[Bulma ref.](http://bulma.io/documentation/form/general/)

**All generic form fields, found at `Symbol > form/field/`**

There are 4 size variants for 2 types of fields :

- **input / select** (change), with or without a *help* element
- **textarea**, with or without a *help* element

The **input** field can be changed to a **select** field through the `input` select on the Overrides panel.

For the icons variants on the input fields, see next section, [Input](#form-input).

**Radio** and **checkbox** fields are also available, though they do not have size variants. They can be used as-is (change the text in the Overrides panel), or if you need styled text (bold, link color…) you have to `Detach from Symbol`.

You can find labels in `Symbol > form/label/`.

File upload inputs haven't been made available as fields.

#### TODO

- Horizontal fields
- Fields with addons (same problem as with [Buttons](#elements-button), re: rectangle radius)

### Input [form-input]

[Bulma ref.](http://bulma.io/documentation/form/input/)

**Text inputs and variants, found at `Symbol > form/control/input/`**

There are 4 size variants, for each of which there is one disabled variant.

The border color can be changed via the `border` select in the Overrides panel.

The text can be changed in the Overrides panel. Because of limitations in Sketch, I have separated the styles for placeholder text and filled text (placeholder text is lighter, filled text is darker, it's the text displayed in the input once you've filled it). In the Overrides panel, filled text is empty and the placeholder has been used.

See the [icon element](#elements-icon) to learn more about changing the icon displayed.


### Textarea [form-textarea]

[Bulma ref.](http://bulma.io/documentation/form/textarea/)

**Multiline textarea control, found at `Symbol > form/control/textarea/`**

There are 4 size variants, for each of which there is one disabled variant.

The border color can be changed via the `border` select in the Overrides panel.

The text can be changed in the Overrides panel. Because of limitations in Sketch, I have separated the styles for placeholder text and filled text (placeholder text is lighter, filled text is darker, it's the text displayed in the input once you've filled it). In the Overrides panel, filled text is empty and the placeholder has been used.

### Select [form-select]

[Bulma ref.](http://bulma.io/documentation/form/select/)

**A styled Select element, found at `Symbol > form/control/select`**

*Multiple select is currently unavailable.*

There are 4 size variants, and one variant in each size with an icon to the left.

The border color can be changed via the `border` select in the Overrides panel.

The text can be changed in the Overrides panel. Because of limitations in Sketch, I have separated the styles for placeholder text and selected text (placeholder text is lighter, selected text is darker, it's the text displayed in the select once you've selected one option). In the Overrides panel, selected text is empty and the placeholder has been used.

See the [icon element](#elements-icon) to learn more about changing the icon displayed.


### Radio [form-checkbox]

[Bulma ref.](http://bulma.io/documentation/form/checkbox/)

**Radio control, found at `Symbol > form/control/checkbox`**

One checked variant is available.


### Radio [form-radio]

[Bulma ref.](http://bulma.io/documentation/form/radio/)

**Radio control, found at `Symbol > form/control/radio`**

One checked variant is available.


### File [form-file]

[Bulma ref.](http://bulma.io/documentation/form/file/)

**Custom file upload input, found at `Symbol > form/control/file/`**

The file upload input exists in 4 size variants, the option to display the file name (left or right), the option to display it boxed, or boxed with the file name. 20 different combinations.

To display an input with the CTA and the name, you have to combine the right `file-cta` to the right `file-name`. E.g.: `form/control/file/default/file-cta has-name` and `form/control/file/default/file-name has-name`



---

## Elements

### Box [elements-box]

[Bulma ref.](http://bulma.io/documentation/elements/box/)

**A simple white box to be found at `Symbol > elements/box`. No variants, nothing else.**

### Button [elements-button]

[Bulma ref.](http://bulma.io/documentation/elements/button/)

**All the buttons can be found at `Symbol > elements/button/`**

The default button is `Symbol > elements/button/default`. There are variants by sizes : `small`, `default`, `medium` and `large`, and there are variants for buttons with icons : `icon`, `icon-left` and `icon-right`.

Each variant can be customised in various ways, through the Overrides panel.

- **type** is used to change the text color through a typography Symbol
- **text** is used to change the text
- **background** is used to change the background color through a color Symbol
- **border-color** is used to change the border color through a color Symbol

When using a derived color (like `Symbol > colors/primary`) you will have another override choice (like `primary color`: `colors/turquoise`). Don’t change it.

Buttons have three variants with icons. Two of them display text and icon (icon to the left or to the right of the text) one displays only an icon in a square button.

See the [icon element](#elements-icon) to learn more about changing the icon displayed.

#### TODO

Button groups with addons. As I can’t use Symbols as masks I can’t make it customisable through overrides, so I have to duplicate all button Symbols to change the border radiuses.

### Content [elements-content]

Currently unavailable.

### Delete [elements-delete]

[Bulma ref.](http://bulma.io/documentation/elements/delete/)

**A delete cross in a semi-transparent circle, available in 4 sizes at `Symbol > elements/delete`**

### Icon [elements-icon]

[Bulma ref.](http://bulma.io/documentation/elements/icon/)

**FontAwesome icons displayed in containers, available at `Symbol > elements/icon`.**

There are 4 container variants, each container has up to 4 size variants, and each size has 8 color variants.

When inserting  an icon element Symbol, you can modify the icon itself through the Override panel. Just paste the icon character, it can only work with FontAwesome icons. The icon character can be found with the Icon Font extension for Sketch.

#### TODO

Would it be wise to get all the icons from FontAwesome as Symbols? I don't think it'd be wise, as there are 4 different sizes (and a few hundred of icons).

### Image [elements-image]

Currently unavailable.



### Notification [elements-notification]

[Bulma ref.](http://bulma.io/documentation/elements/notification/)

**A simple notification to be found at `Symbol > elements/notification`**

There are two Symbols for this element. The background and the complete notification.

How to use? Insert `Symbol > elements/notification/notification` and change the text through the Overrides panel. If you need bold & links, you'll have to *Detach from Symbol* so you can edit the text. The rest of the group will be the `notification-layout` Symbol.

### Progress [elements-progress]

[Bulma ref.](http://bulma.io/documentation/elements/progress/)

**A progress bar, found at `Symbol > elements/progress`. Exists in 4 sizes.**

You can change the colors of the progress and the background through the Overrides panel. If you need to change the progress width, you'll have to *Detach from Symbol*.


### Table

Currently unavailable.


### Tag

[Bulma ref.](http://bulma.io/documentation/elements/tag/)

**Small tag labels, found at `Symbol > elements/tag`**

There are 3 size variants, 3 addon variants (no addon, left-side addon or right-side addon), and 1 round border alternative for each of these variants.

There is also an alternative where a tag has a delete button, and an alternative where a tag is a delete button to be used as a right-side addon.

Each of these Symbols can be customised via the Overrides panel :

- **type** to change text color via a typography Symbol
- **text** to change the text
- **background** to change background color via a color Symbol
- **delete** if it's `has-delete` tag type, not really an useful override




### Title

[Bulma ref.](http://bulma.io/documentation/elements/title/)

**Page headings, found in the `Styled Text` submenu.**

#### TODO :

Should I make Symbols for title/subtitle groupings? The right margin could be useful.

---

## Components

### TODO :

Everything

