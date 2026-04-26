# ✨ Timetable Planner

A fun, interactive drag-and-drop school timetable builder for kids. Built as a single self-contained HTML file — no installation, no server, no dependencies.

![Pink timetable builder with drag and drop subjects](https://placehold.co/800x400/fff0f7/d4186a?text=✨+Timetable+Builder)

## Features

- 🎨 **Drag and drop** subjects onto your timetable, or tap to select then tap a cell
- 💾 **Save and load** timetables per person — each friend gets their own saved slot
- 🖨️ **Print-ready** — full colour A4 landscape output, UI chrome hidden automatically
- 🌸 **Personalised** — enter your name, pick a Week 1 / Week 2 / both layout, and choose an avatar
- 📚 **16 subjects** included: Maths, English, Science, History, Geography, PE, Art, Music, Tech, Spanish, German, French, Computing, Drama, RE, PSHE
- 📱 **Mobile friendly** — works on phones and tablets as well as desktop

## Getting Started

### Use it instantly

Just open `index.html` in any modern web browser. No installation required.

### Host on GitHub Pages

1. Fork or clone this repo
2. Go to **Settings → Pages**
3. Set Source to **Deploy from branch → main**
4. Your app will be live at `https://pucbaldwin.github.io/timetableplanner`

## How to Use

1. **Enter your name** and pick your avatar and which week(s) you want
2. Click **Build My Timetable!**
3. **Drag a subject** from the palette at the top onto any lesson slot — or tap a subject to select it, then tap a cell
4. Click the **×** on any cell to remove a subject
5. Hit **💾 Save** to save your timetable — it will appear on the home screen next time
6. Hit **🖨️ Print** to print in full colour

## Saving & Loading

Timetables are saved in the browser's `localStorage`. This means:

- ✅ Saves persist between sessions on the same device and browser
- ✅ Multiple people can each have their own saved timetable
- ❌ Saves do not sync between devices

## Printing Tips

- Click **🖨️ Print** inside the app (don't use the browser's File → Print directly)
- In the print dialog, enable **Background graphics** under More Settings to get full colour
- Output is formatted for **A4 landscape**

## Tech Stack

| | |
|---|---|
| Languages | HTML, CSS, vanilla JavaScript |
| Fonts | [Baloo 2](https://fonts.google.com/specimen/Baloo+2) + [Quicksand](https://fonts.google.com/specimen/Quicksand) via Google Fonts |
| Storage | Browser `localStorage` |
| Dependencies | None |

## File Structure

```
timetableplanner/
└── index.html    # The entire app — HTML, CSS and JS in one file
```

## Customising

Want to add or remove subjects? Find the `SUBJECTS` array near the top of the `<script>` block in `index.html`:

```javascript
const SUBJECTS = [
  { id:'maths',   name:'Maths',   emoji:'🔢' },
  { id:'english', name:'English', emoji:'📖' },
  // Add your own here...
  { id:'latin',   name:'Latin',   emoji:'🏺' },
];
```

Each subject also needs a colour pair added to the CSS — search for `chip-maths` to see the pattern.

## License

MIT — free to use, share and modify.

---

Made with 🌸 for Maya and friends.
