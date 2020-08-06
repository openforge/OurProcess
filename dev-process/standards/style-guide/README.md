# Openforge Style Guide

## Table of Contents

1. [CSS Basic Rules](#css-basic-rules)
2. [SCSS Basic Rules](#scss-basic-rules)
3. [Learning Resources](#learning-resources)
4. [Style Resources](#style-resources)

## CSS Basic Rules

- Use CSS Variables for colors instead of just using RGB, RGBA or HEX code. CSS Variables should be defined in the `:root` under variables CSS file. This will help in the future to update colors easily.
- The repeated CSS code should go in the global CSS file with a specific class name in order to point those individual elements that are using that repeated code.
- The structure of the CSS classes should match the HTML structure in order to make it easier to find an exact piece of code.
- Avoid the usage of ID unless it is trully needed.

## SCSS Basic Rules

- Use SCSS Variables for colors instead of just using RGB, RGBA or HEX code. SCSS Variables should be defined in the `:root` under variables SCSS file. This will help in the future to update colors easily.
- The repeated SCSS code should go in the global SCSS file with a specific class name in order to point those individual elements that are using that repeated code.
- The structure of the SCSS classes should match the HTML structure in order to make it easier to find an exact piece of code.
- Avoid the usage of ID unless it is trully needed.
- Avoid more than 3 levels deep on the SCSS files in favor of readability and not rely to much on HTML structure that is fragile.
- Avoid to write a nested SCSS block with more than 50 lines cause will be harder to read and difficult to understand.

## Learning Resources

This list is filled with helpful links in order to learn more about CSS patterns. Right now is just for learn Grid and Flexbox.

1. [CSS Grid](https://css-tricks.com/snippets/css/complete-guide-grid/)
2. [CSS Flex](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)

## Style Resources

This list is filled with some great resources links in order to generate CSS / SCSS code for especific needs. You can find here from a page that helps you generating your background gradients to a page that generates you loading spinners!

1. [Box Shadow](https://www.cssmatic.com/box-shadow)
2. [CSS Gradient](https://www.colorzilla.com/gradient-editor/)
3. [Other CSS Gradient](https://cssgradient.io/)
4. [CSS Section Separator](https://wweb.dev/resources/css-separator-generator)
5. [Loading Spinners](https://loading.io/)
6. [SVG Waves](https://getwaves.io/)
