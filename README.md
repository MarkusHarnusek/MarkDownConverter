# MarkDown Converter

## What is the MarkDown Converter?
The MarkDown Converter is a web-based tool designed to convert Markdown files into styled HTML documents. It simplifies the process of transforming plain text Markdown into visually appealing web pages. All regular MarkDown Signature are implemented alongside custom signatures.

## Custom Features

- **Image Scaling**: Customize image sizes effortlessly using the enhanced syntax: `![Alt](url)(<scale-factor>)`. This feature extends the standard Markdown image syntax to include scaling capabilities.

- **Message Blocks**: Highlight and categorize important information with structured message blocks, consisting of headers and body tags. The following block types are available:
  - **Info Block**: Use `#ih` for the header and `#ib` for the body to provide additional information.
  - **Positive Block**: Use `#+h` for the header and `#+b` for the body to emphasize positive actions or recommendations (e.g., Do's).
  - **Warning Block**: Use `#wh` for the header and `#wb` for the body to draw attention to critical warnings.
  - **Negative Block**: Use `#-h` for the header and `#-b` for the body to highlight negative actions or cautions (e.g., Don'ts).

- **Calculations**: Wrap calculations in `#cal` tags to create custom-styled calculation elements.

- **Enhanced Code Blocks**: Create visually appealing code blocks with line numbers, syntax highlighting, and a copy-to-clipboard button. Simply enclose your code with `#codefs(<programming-language>)` and `#codefe` tags.

## How to Import and Use
1. Clone the repository to your local machine.
2. Include the stylesheet and import the script as a module in the `.html` file:
    ```html
    <link rel="stylesheet" href="./styles/markdown-styles.css"/>
    <script type="module" src="./scripts/md-converter.js"></script>
    ```
3. Import `markdown-converter` in your script:
    ```javascript
    import MarkdownConverter from "./md-converter.js";
    ```
4. Use the `markdownConverter` function to convert Markdown to HTML:
   ```javascript
   const markdownContent = `# Hello World!`;
   const htmlContent = markdownConverter(markdownContent);
   document.body.innerHTML = htmlContent;
   ```

## Q&A

**Q: Can I use custom fonts?**
A: Yes, you can add your own fonts to the `assets/fonts` directory and update the CSS file to incorporate them into your project.

**Q: Does it support images?**
A: Yes, the converter fully supports images. Simply include them in your Markdown, and they will be rendered seamlessly in the HTML output.

**Q: Are themes supported?**
A: Yes, the Markdown Converter comes with built-in support for both dark and light themes. Comprehensive documentation on CSS variables is provided, allowing you to customize the themes to suit your needs.

**Q: Can it load Markdown files?**
A: Yes, you can use the `loadMarkdown(path)` function to load and convert Markdown content directly from a file.

## Usage and Licensing

The Markdown Converter is a powerful tool to streamline your Markdown-to-HTML workflows. While using this tool, please ensure compliance with the [CC BY 4.0 License](./LICENSE) by providing proper attribution as required.

## Feedback and Contributions

I value your feedback and contributions to improve the Markdown Converter! If you encounter any issues, have suggestions, or want to request new features, please feel free to open an issue in the repository. Contributions are also welcome—whether it's fixing bugs, adding new features, or improving documentation.

## Credits

### Co-Authoring

Some style aspects have been codeveloped by [7XDev](https://github.com/7XDev)

### Icons
#### Flaticon Icons
- [Camera drone icons created by vectorsmarket15 - Flaticon](https://www.flaticon.com/free-icons/camera-drone)
- [Next icons created by Roundicons - Flaticon](https://www.flaticon.com/free-icons/next)
- [Ui icons created by shin_icons - Flaticon](https://www.flaticon.com/free-icons/ui)
- [Mode icons created by amoghdesign - Flaticon](https://www.flaticon.com/free-icons/mode)
- [Dark icons created by adriansyah - Flaticon](https://www.flaticon.com/free-icons/dark)
- [Wrong icons created by I Wayan Wika - Flaticon](https://www.flaticon.com/free-icons/wrong)

#### FontAwesome Icons
- [Triangle Exclamation](https://ka-p.fontawesome.com/releases/v6.6.0/svgs/regular/triangle-exclamation.svg?v=2&token=a463935e93)
- [Circle Check](https://ka-p.fontawesome.com/releases/v6.6.0/svgs/regular/circle-check.svg?v=2&token=a463935e93)
- [Circle Info](https://ka-p.fontawesome.com/releases/v6.6.0/svgs/regular/circle-info.svg?v=2&token=a463935e93)
