# Responsive Course Page

A responsive HTML and CSS course page built with Flexbox, Grid and media queries.
Task 8 of my Bloomrix internship. No JavaScript is used.

## Files
- index.html - the page
- style.css - all the styling
- images/ - the photos used on the page

## Layout systems
- Flexbox: header and navigation, hero, card bodies, form rows
- Grid: course cards, lesson layout, course summary cards, footer

## Responsive approach
The styles are mobile-first. The base CSS is for small screens. Two min-width media queries
add changes: 768px (tablet) and 1024px (desktop).
- 768px: the header and the hero become rows, and the footer gets two columns.
- 1024px: the lesson sidebar moves to the right, and the footer gets four columns.
The card grids use repeat(auto-fit, minmax()), so they change their number of columns by
themselves without a media query.

## Responsive typography
The headings use clamp(), so they grow and shrink smoothly between a minimum and a maximum
size. The page width uses min() and the side padding uses max().

## Focus styles
I do not remove outlines. :focus-visible gives links, buttons and fields a clear amber
outline for keyboard users. Removing an outline without a replacement makes it impossible
for people who use the Tab key to see where they are.

## Transitions and transforms
Navigation links, buttons, course cards, card images and summary cards use a transition with
a transform (scale, translate or rotate).

## Tested widths
Mobile 375px, tablet 768px and desktop 1280px, checked in browser DevTools.

## How to run
Open index.html with Live Server in Visual Studio Code, or in any web browser.