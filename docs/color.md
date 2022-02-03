# Colors
Colors are categorized into the areas: `text & icon`, `background`, `primary`, `ui`, `functional` and `additional`.

## Text & icons
`Text & icon` tokens should be exclusivly used as text colors and icon colors. Text and icons have very specific contrast needs to fulfill accessibility requirements.
By combining the correct background and `Text & icon` tokens you can be assure that contrast ratios requirements are fulfill. 
In the color table you find the accepted combinations with the resulting contrast rating.
### Standard
`Text & icon/Standard` is the main text token used for headlines, copy text and important ui texts & labels.

### Additional
`Text & icon/Additional` is used for additional content that should be a bit de-emphasized. It is also used for placeholder texts, labels within text fields or unselected elements.

### Disabled
`Text & icon/Disabled` is exclusivly used for text and icons of disabled elements. It does not fulfill the contrast ratio for active text, however for disabled elements it is acceptable to not fulfill the contrast according to [wacg specifications; incidental](https://www.w3.org/WAI/WCAG21/Understanding/contrast-minimum).

### Link
The `Text & Icon/Link` tokens should be used exclusivly for links and the link underline. Make sure to use the correct tokens for the link states `standard`, `hover`, `visited`, `active`.

### Primary
The `Text & Icon/Primary` tokens are used for text of specific interactive components like active menu item.

### Functional
#### Informational, Success, Warning & Danger
These tokens are for text in specific situations:
- `Text & icon/Functional/Informational` is for neutral information, like an update of the terms of service.
- `Text & icon/Functional/Success` is for confirmation messages of successfully performed actions.
- `Text & icon/Functional/Danger` is for errors or confirmation texts for dangerous choice like deleting an account. It may also be used for destrutive actions like _delete_.
- `Text & icon/Functional/Warning` is for warning messages about potential problems or inconvenient circumstances like a planned outage for maintainence.

#### White & Black
The tokens `Text & icon/Functional/White` & `Text & icon/Functional/Black` are the same colors as the standard colors. The difference is that the color will **not** change between light and dark mode.
This means `Text & icon/Functional/White` is white in light **and** dark mode and `Text & icon/Functional/Black` is black in light **and** dark mode.
Only use those colors were nessesary, e.g. on functional colors or the primary color.

### Inverted
`Text & icon/Inverted/Standard` & `Text & icon/Inverted/Additional` are the exact opposites of the `Text & icon/Standard` and `Text & icon/Additional`. Their actual color depends on the current mode.

When you are using *light mode* the standard text color is *black*, so the opposite, `Text & icon/Inverted/Standard` is *white*.
Conversly when you are using *dark mode* the standard text color is *white*, so the opposite, `Text & icon/Inverted/Standard` is *black*.

When do you need the inverted colors? Only in very specific cases. For example when you want to put text on top of `ui/strong` and `ui/extra strong`.

## Background
`Background` tokens are used for big background areas on which other components are place.

### Canvas
`Background/Canvas` & `Background/Canvas Subtle` tokens are only used for the background of an app or website.
### Surface
`Background/Surface`, `Background/Surface Subtle` & `Background/Surface Highlight` tokens are used for bigger elements like cards, modals, header or footers that are above the canvas but often contain components.

### Backdrop
The `Background/backdrop` token is used for an overlay that covers the screen below a modal window or similar.

## Primary
`Primary` tokens are used for important parts of the product. This includes the primary action button, an active item in a ui element like a checkbox or an active tab or an enabled element like a toggle switch.
The state tokens `hovered` and `pressed` should only be used to visualize these specific interaction states.
## UI
`UI` tokens are used for borders and backgrounds and parts of ui components like buttons, sliders, switches, inputs, etc.

### Base
The `ui/base` token is used for parts of ui elements that are same / similar in color to the background. For example the knob in a switch or slider.
It may also be used for other purposes that are not covered by any of the other ui colors.

### Subtle
The `ui/subtle` token is mainly used when a background for a ui element is needed that is supposed to have only little contrast to the apps background. It does not fulfill the wacg contrast requirements of 3:1 for ui elements so it should not be used as the only means to visualize a ui element or for important functional aspects. 
It may also be used for other purposes that are not covered by any of the other ui colors.

### Light
The `ui/light` token is mainly used for decorational aspects of ui elements. It does not fulfill the wacg contrast requirements of 3:1 for ui elements so it should not be used as the only means to visualize a ui element or for important functional aspects.
It may also be used for other purposes that are not covered by any of the other ui colors.

### Regular
The `ui/regular` token is used for the main part in many ui elements in the default state. E.g. for the outline of an input field or radio button.
It may also be used for other purposes that are not covered by any of the other ui colors.

### Strong
The `ui/strong` token is used for hover effects, e.g. when a radio button is hovered the outlien changes from `ui/regular` to `ui/strong`.
It may also be used for other purposes that are not covered by any of the other ui colors.

### Extra Strong
The `ui/extra-strong` token is used for pressed effects and when a very strong contrast is needed, e.g. when a radio button is pressed the outlien changes from `ui/regular` to `ui/extra-strong`.
It may also be used for other purposes that are not covered by any of the other ui colors.

### Disabled
The `ui/disabled` token should be used together with the `Text & icon/Disabled` token to create disabled elements. This token must only be used for disabled elements.

## Functional
`Functional` tokens are for specific situation in which they are applied.

### Focus
The `Functional/Focus` token is exclusivly used for the focus ring when navigating with tab or a remote.

### Informational
The `Functional/Informational` tokens are for informative elements like info banners or specific interactive elements like progress bars or sliders.

### Success
The `Functional/Success` tokens are for success elements like confirmation banners or success states, like an outline for an input field with a valid credit card number.

### Danger
The `Functional/Danger` tokens are for errors states like the outline of an invalid text field or a dangerous choice like a deletion button.

### Warning
The `Functional/Warning` tokens are for warnings like a progress bar of data usage that is nearly filled.

## Additional
`Additional` tokens must only be used for specific elements where colors server a more decorational purpose and don't have a semantic meaning.
Some examples are tags or bar charts & graphs.
