# AI Prompt Library - Setup Instructions

## Quick Start
1. Download both files: `index.html` and `config.json`
2. Put them in the same folder
3. Open `index.html` in your web browser
4. To customize, edit `config.json` using any text editor

## How to Customize (No Coding Required!)

### Editing the Configuration File

Open `config.json` in any text editor (Notepad, TextEdit, etc.) and modify the content:

#### Adding a New Category
```json
{
  "name": "Your Category Name",
  "icon": "🎯",
  "subtitle": "Description of what this category contains",
  "snippets": [...]
}
```

#### Adding a New Prompt Snippet
```json
{
  "title": "Your Prompt Title",
  "content": "Your prompt text goes here.\n\nUse \\n\\n for line breaks.\nUse [PLACEHOLDERS] for things users should replace."
}
```

#### Adding an Alternative Version
```json
{
  "title": "Main Prompt Title",
  "content": "Main prompt content here",
  "alternative": {
    "title": "Alternative Title (optional)",
    "content": "Alternative prompt content here"
  }
}
```

### Tips for Writing Good Prompts

1. **Use [PLACEHOLDERS]** for things users need to customize:
   - `[TOPIC]` for the subject matter
   - `[WORD COUNT]` for length requirements
   - `[YOUR NAME]` for personalization

2. **Include clear instructions** in your prompts:
   - What information the user needs to provide
   - What format they want the output in
   - Any specific requirements

3. **Use line breaks** (`\n\n`) to organize your prompts:
   - Separate different sections
   - Make instructions easier to read

4. **Test your prompts** with AI tools to make sure they work well

### Icons for Categories
Copy and paste these emoji icons:
- 📚 (books) - Academic/Education
- 💼 (briefcase) - Business/Professional
- 🎯 (target) - Goals/Planning
- 💬 (speech) - Communication
- 🎨 (art) - Creative
- 🔧 (wrench) - Technical/Tools
- 📊 (chart) - Analytics/Data
- 🏠 (house) - Personal/Home
- 🌟 (star) - Featured/Popular
- ❓ (question) - Help/Support

### Common Issues

**"Error loading configuration"**
- Make sure `config.json` is in the same folder as `index.html`
- Check that your JSON syntax is correct (use a JSON validator online)
- Make sure all quotes are straight quotes (" not " or ")

**Content not showing up**
- Check for missing commas between sections
- Make sure all brackets { } are properly closed
- Use `\n` for single line breaks, `\n\n` for paragraph breaks

**Alternative button not working**
- Make sure your alternative section is properly formatted
- The alternative content should be inside an "alternative" object

### Example of a Complete Category

```json
{
  "name": "Writing Help",
  "icon": "✍️",
  "subtitle": "Prompts to help with various writing tasks",
  "snippets": [
    {
      "title": "Blog Post Creator",
      "content": "Write a blog post about [TOPIC].\n\nTarget audience: [WHO READS THIS]\nTone: [PROFESSIONAL/CASUAL/FUNNY]\nLength: [WORD COUNT] words\n\nPlease include:\n• Catchy headline\n• Engaging introduction\n• 3-5 main points\n• Strong conclusion\n• SEO-friendly subheadings"
    },
    {
      "title": "Email Template",
      "content": "Help me write an email for [PURPOSE].\n\nRecipient: [WHO]\nTone: [FORMAL/FRIENDLY]\nMain request: [WHAT YOU NEED]\n\nPlease provide a professional email with subject line.",
      "alternative": {
        "title": "Quick Email",
        "content": "Write a short email to [PERSON] asking for [REQUEST]. Keep it brief and polite."
      }
    }
  ]
}
```

### Hosting Your Site

1. **Local use**: Just open `index.html` in your browser
2. **Online hosting**: Upload both files to any web hosting service
3. **GitHub Pages**: Upload to a GitHub repository and enable Pages
4. **Simple hosting services**: Netlify, Vercel, or similar services

### Updating Your Library

1. Edit `config.json` with your changes
2. Save the file
3. Refresh your browser to see updates
4. No need to touch the HTML file unless you want to change colors/styling

Need help? Most issues are related to JSON formatting. Use an online JSON validator to check your config.json file if something isn't working.
