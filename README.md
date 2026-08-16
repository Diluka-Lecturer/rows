# Flutter Lab: Rows and Alignment

In this lab, you will learn how to use the `Row` widget to arrange multiple widgets horizontally across the screen. You will also see how the layout axes behave differently than they did in the `Column` lab.

## Understanding the Axes in a Row
- **Main Axis (Horizontal):** Controlled by `mainAxisAlignment`. It determines how space is distributed left-to-right (e.g., clustered at the start, spread evenly, pushed to the end).
- **Cross Axis (Vertical):** Controlled by `crossAxisAlignment`. It determines how children align top-to-bottom within the row (e.g., centered, aligned to the top/start, or bottom/end).

## Prerequisites
1. Clone this repository to your local machine.
2. Run `flutter pub get` in your terminal.
3. Launch an emulator or connect a physical device, and run the app. 

## Instructions
Open `lib/main.dart` and locate the `TODO` comments inside the `body` of the `Scaffold`.

1. **Add Children**: Inside the `children` list of the `Row`, replace the placeholder text with three new widgets: a `Text` widget, an `ElevatedButton` (styled with a red background), and a `Container` (styled with a cyan background, padding of 30, and text inside).
2. **Main Axis Alignment**: Notice how your widgets are bunched up on the left side of the screen. Add the `mainAxisAlignment` property to the `Row` to spread them out evenly from left to right.
3. **Cross Axis Alignment**: Add the `crossAxisAlignment` property to push all the widgets to the bottom (the "end" of the cross axis). Notice how the smaller widgets align their bottom edges with the bottom edge of the tallest widget (your Container).

## Expected Output
When completed, you should see your three widgets distributed evenly across the screen horizontally. Because you set the cross-axis alignment to the end, the bottom edges of the text, button, and container will all line up perfectly.
